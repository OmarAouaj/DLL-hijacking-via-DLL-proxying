# Pre-Compiled DLLs for Hijacking Tests

- Are you testing a thick client application for **DLL hijacking**?
- Did you launch the application and search for DLLs in writable directories that are **"NOT FOUND"**?
- Feel too lazy to run Spartacus and manually export functions from benign DLLs?

If you answered **yes** to all of the above — this repository is for you.

## 🔧 What’s Inside

This repository provides **pre-compiled DLLs** that:
- Export the required functions from benign Windows DLLs
- Display a **MessageBox** as a **Proof of Concept (PoC)** for your penetration test reports

These DLLs are ready to drop into your testing directory — no need to compile or export anything yourself.

## 📥 Download

You can download the latest precompiled DLLs from the [Releases](../../releases) section of this repository.

> 🔄 Releases will be updated regularly with new DLLs as they become available.

## 📌 Use Case

Useful during:
- DLL hijacking assessments
- Thick client security testing
- Quick and easy PoC demonstrations

## 🧠 Tips

- In some cases, you can reuse a malicious DLL by simply renaming it.  
  For example, if you have a malicious version of `netapi32.dll`, you might be able to reuse it as `profapi.dll` **by renaming the file**.

> ⚠️ This only works if the application calls **functions with matching exports**.  

## ⚠️ Note on Antivirus Detection

> These precompiled DLLs may be flagged by antivirus solutions.  
> This is expected, as the MessageBox payload was generated using **msfvenom**, which is commonly detected.  
> **They are intended strictly for PoC purposes in controlled environments.**

Future versions will aim to include less detectable binaries while preserving the demonstration purpose.

## 🛑 Disclaimer

These DLLs are for **educational** and **penetration testing purposes** only. Use them responsibly and only with proper authorization.

---

Contributions and suggestions are welcome!
