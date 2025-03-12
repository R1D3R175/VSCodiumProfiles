# Security Policy
Sometime it may happen that an extension obfuscates malicious code *good enough* to bypass automated checks; while I try to make sure the extensions *aren't* malicious, we are all humans and it just happens; take for example the `xz-utils` case. 

## Reporting a security bug
If an extension (or whatever third-party software the VS Codium profiles use) has been **proven** to contain malicious code and hasn't yet been removed from the [Open VSX Registry](https://open-vsx.org/) (or whatever third-party software source the VS Codium profiles use), please open an issue stating which profile is affected and in what way, if possible also include methods to fix the issue and/or remove whatever persistency the malicious code has (if applicable).

## Security Recommendations
If you have a *reasonable suspect* that an extension may be malicious, report it to the maintainer(s) of the third-party software following their security guidelines. Don't report it here as you could *accidentally* **disclose** a vulnerability when it *hasn't been fixed yet*. 

If you want, you can still reach me via GitHub's no reply email <54753989+R1D3R175 at users dot noreply dot github dot com> and we can discuss if and how the extension should be removed from the affected profiles without disclosing anything. Note that you don't have to (and probably neither should) tell me the details of the vulnerability.
