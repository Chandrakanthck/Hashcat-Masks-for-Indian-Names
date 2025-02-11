# Hashcat Masks for All Indian Names

This repository contains a collection of **Hashcat masks** generated from Indian names.
These masks can be used for password cracking research, security analysis purposes.

## Files Included

- `mask_1_placeholder.txt`: Hashcat masks with 1 placeholder.
  - This represents the most possible passwords based on Indian names.
- `mask_2_placeholders.txt`: Hashcat masks with 2 placeholders.
- `mask_3_placeholders.txt`: Hashcat masks with 3 placeholders.
- `mask_4_placeholders.txt`: Hashcat masks with 4 placeholders.
- `mask_5_placeholders.txt`: Hashcat masks with 5 placeholders.
- `mask_6_placeholders.txt`: Hashcat masks with 6 placeholders.
- `all_masks_combined.txt`: All masks combined into one file.
- `mask_4_5_6_placeholders.txt`: Masks for placeholders 4, 5, and 6.

## How to Use

### Using Hashcat with the Provided Masks

You can use these masks in **Hashcat** for password cracking by specifying the mask file. Modify the settings according to your needs, such as the hash type and the custom charset (?1).

### Example Command:

```sh
hashcat -m 0 -a 3 hash.txt mask_1_placeholder.txt --force
```

### Using executemask.bat

A batch file (`executemask.bat`) is included to automate the Hashcat execution process. It reads masks from `masks.txt` and runs them against the hash file.

#### Configuration:

- **Hash file:** Change `hash.hc22000` to your actual hash file. Example:
  ```sh
  set HASH_FILE=myhashes.txt
  ```
- **Attack mode and hash type:** Modify `-m 22000` for WPA hashes. If using other hash types, use the appropriate mode:
  - MD5: `-m 0`
  - SHA-1: `-m 100`
  - SHA-256: `-m 1400`
  - SHA-512: `-m 1700`
  - CRC32: `-m 11500`
  - XXH32: `-m 16200`
  - XXH64: `-m 16210`
- **Custom charset (?1):** Change `0123456789!@#_.*` if needed. Example:
  ```sh
  set CHARSET=-1 abcdefghijklmnopqrstuvwxyz0123456789!@#%_.*&
  ```

Run the batch file by double-clicking `executemask.bat` or using:

```sh
cmd /c executemask.bat
```

The script will attempt all masks and stop if a password is cracked. The cracked password (if found) will be saved in `cracked.txt`. 🚀

You can now download the files individually from this repository on GitHub! 🚀
