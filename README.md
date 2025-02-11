# Hashcat Masks for All Indian Names

This repository contains a collection of **Hashcat masks** generated from Indian names.
These masks can be used for password cracking research, security analysis purposes.

## Files Included

- `output_1.txt`: Hashcat masks with 1 placeholder.
  - This represents the most possible passwords based on Indian names.
- `output_2.txt`: Hashcat masks with 2 placeholders.
- `output_3.txt`: Hashcat masks with 3 placeholders.
- `output_4.txt`: Hashcat masks with 4 placeholders.
- `output_5.txt`: Hashcat masks with 5 placeholders.
- `output_6.txt`: Hashcat masks with 6 placeholders.
- `combined_output.txt`: All masks combined into one file.
- `output_4_5_6.txt`: Masks for placeholders 4, 5, and 6.

## How to Use

You can use these masks in **Hashcat** for password cracking by specifying the mask file.
Example command:

```sh
hashcat -m 0 -a 3 hash.txt output_1.txt --force
```

## How to Clone and Push to GitHub

To upload this project to GitHub, follow these steps:

1. Initialize Git:

```sh
git init
```

2. Add the files:

```sh
git add .
```

3. Commit the files:

```sh
git commit -m "Initial commit - Added Hashcat masks for Indian names"
```

4. Create a GitHub repository [here](https://github.com/new) and get the repository URL.

5. Add the remote origin:

```sh
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

6. Push the files:

```sh
git branch -M main
git push -u origin main
```

You can now access these files on GitHub and use them for password cracking research.

