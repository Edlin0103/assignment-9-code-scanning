# Answers to Part 3

Add your answers to the questions in Part 3, Step 2 below. 

## Vulernability Remediation:
### Vulnerability 1: 
1. Which package or library are you addressing?
The PyYAML Python library.(scout resulats)

2. Which CVE is linked to this vulnerability?
CVE-2020-14343

3. What remediation steps do you suggest?
The markdown informed that for PyYAML versions before 5.4, it is susceptible to arbitrary code execution when it processes untrusted YAML files through the full_load method or with the FullLoader loader. Update PyYAML version to 5.4 or later and use safe_load() instead of unsafe loaders.

### Vulnerability 2:
1. Which vulnerability are you addressing?
PyYAML enables arbitrary command execution through unsafe YAML deserialization.

2. Which CVE is linked to this vulnerability?
CVE-2020-1747

3. What remediation steps do you suggest? 
Update PyYAML to versions after 5.3.1, better upadte to versions after 5.4 considering the first vulernability and use safe_load(). The two vulernability affect the same library, but the second one seems to be the earlier flaw that CVE-2020-14343 tried to fix completely.
