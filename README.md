# NETWORKWALKS-AHMED-SAMEH-ABDELKADER-B083C-WK3-PM2-Password-Cracking

## Task
Crack the password of 3 encrypted PDF files using the Networkwalks Hash Calculator and Password Cracker tools (dictionary attack), then verify with John the Ripper (Johnny GUI) and the Online HashCrack PDF hash extractor.

## Steps
1. Uploaded each locked PDF to the Networkwalks Hash Calculator to extract the `$pdf$...` hash (pdf2john / hashcat compatible format).
2. Pasted each hash into the Networkwalks Password Cracker (dictionary attack, 100-word built-in list).
3. Ran the attack for each hash until a match was found.
4. Opened each PDF with the cracked password to confirm and capture the flag.
5. Cross-verified the hash extraction using Online HashCrack's PDF Hash Extractor tool, and set up John the Ripper (Johnny GUI) locally as an alternative cracking method.

## Results

| File | Hash (truncated) | Cracked Password | Flag |
|---|---|---|---|
| My-Locked-PDF1.pdf | $pdf$4*4*128*-1060*1*16*55d1a5c14175da...ef81af1 | password1 | `nw{networkwalks_flag1_jtr_270521_1}` |
| My-Locked-PDF2.pdf | $pdf$4*4*128*-1028*1*16*0853f2cde0ef15...ef81af1 | password1 | `nw{networkwalks_persistence_jtr_270521}` |
| My-Locked-PDF3.pdf | $pdf$4*4*128*-1028*1*16*34eb542eff4e1b...2ab02 | 1qaz2wsx | `nw{networkwalks_flag_260821_1}` |

## Tools Used
- Networkwalks Hash Calculator (networkwalks.com/hash-calculator)
- Networkwalks Password Cracker (networkwalks.com/password-cracker)
- Online HashCrack — PDF Hash Extractor (onlinehashcrack.com)
- John the Ripper (Johnny GUI, John 1.9.0-jumbo-1 win64)

## Key Takeaway
Weak/common passwords (password1, 1qaz2wsx) are cracked in seconds via dictionary attacks. This demonstrates why strong, unique passwords are essential for protecting sensitive documents.
