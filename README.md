# Powershell-Password-Paper

**Purpose**  
Generates a one-time password (secret) composed of a random color, UK city/town, and animal, then creates a local HTML file that securely displays the secret. The HTML page features a click-to-reveal mechanism and a dynamic countdown timer until expiration.

**Key Features**  
- **Secret Generation:** Randomly combines predefined lists of colors, UK cities/towns, and animals to form a unique secret.  
- **AES Encryption:** Encrypts the generated secret to enhance security and decrypts it when the HTML viewer is loaded.  
- **Local HTML Viewer:** Creates a local HTML file with a click-to-reveal interface and an auto-updating countdown timer that hides the secret once expired.  
- **Input Validation:** Prompts the user for a valid positive integer for expiration time and ensures the uniqueness of each secret identifier.  
- **Activity Logging:** Records secret generation, storage, and viewing events to a log file in the temporary folder for auditing purposes.

**Usage**:
```powershell
# Execute the script to generate a secret and launch the local HTML viewer
.\Create-PassPaper.ps1 -Verbose
```

Follow the interactive prompts to set the expiration time and add additional secrets if needed.
