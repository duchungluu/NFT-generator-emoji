# How to run

- `npm install --force`
- `npm run generate`

## png+metadata will be in build/

- `npm uninstall node-fetch`
- `npm install node-fetch@2`

### Any sort of "path" error

Ensure that your layer names in the `config.js` file match exactly to your layer folder names. Also, remove any `-` (hyphens) from your file names.

### "Quota Limit Reached" or "Too many requests" errors

There have been some changes made to the code from the original video resulting from some errors when uploading files, metadata, and minting using NFTPort. Depending on your plan, Free vs Community, there are rate limits.

To fix these issues, I've updated the code to include a timeout that will allow the files to be uploaded at a slower rate, instead of all at once, eliminating these errors.

**To use this code:**

- Clone this repo or download the latest release zip file.
- Unzip, if needed, and open the folder in VS Code.
- From the terminal type:
  - `npm install`
- Copy your image layers into the `layers` folder.
- Use the `src/config.js` file to set up your layers and NFT information.
