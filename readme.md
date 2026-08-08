# DIY Camera Filter Generator (Offline Edition)

A fully offline, browser-based tool to create, edit, and preview custom color filters for digital cameras. 

This project was extracted from a semi-local web tool and modified using AI to completely remove all online/cloud dependencies. It allows you to generate filter files (`.pro`, `.air`, `.dld`) entirely locally on your machine without relying on a website, internet connection, or server.

## 📷 Supported Cameras
* **Pro Series (`.pro`)**: D53, D50, D80, V08 Pro
* **Air Series (`.air`)**: D72, DC08
* **Legacy/Standard (`.dld`)**

## ✨ Features
* **100% Offline**: No tracking, no server uploads, and no external dependencies.
* **Live Preview**: See how your filter affects an image in real-time.
* **Granular Controls**: Adjust Exposure, Contrast, Saturation, Tone (Hue), and individual RGB Gamma curves.
* **Load & Edit**: Import existing `.pro`, `.air`, or `.dld` files to tweak them.
* **Presets**: Quick-start presets for Standard, Highlight, Retro, and B&W.

## 🚀 How to Use

1. **Download/Clone** this repository to your local machine.
2. **Open the HTML file** (e.g., `DIY-Camera-Filters-Offline-Complete`) directly in your web browser (Chrome, Firefox, Safari, Edge).
3. **Upload an Image**: Because this tool runs completely locally (`file://`), modern browsers block canvas manipulations on the pre-loaded thumbnails for security reasons. Click **"Change Picture"** and upload a photo from your computer to use as a preview base.
4. **Select your Camera Model** from the dropdown.
5. **Adjust the Sliders** until you are happy with the preview.
6. Click **"Download Filter (.pro/.air)"** to save the filter to your computer.

### Installing on your Camera
1. Copy the downloaded `.pro` or `.air` file to the root directory of your camera's SD card.
2. Turn on the camera. You should briefly see a "LOAD" message on the screen.
3. *Note: Most cameras can only load one custom file at a time.*

## 🛠️ Technical Details (Offline Verification)
This tool has been heavily modified for offline integrity:
* All CSS and JavaScript dependencies (including jQuery and filter algorithms) have been localized.
* File exports are handled entirely client-side using JavaScript `Blob` objects.
* File imports are handled via the HTML5 `FileReader` API.
* Unnecessary cloud-upload UI elements and telemetry features have been disabled and hidden.

## ⚠️ Disclaimer & Liability

**USE AT YOUR OWN RISK.** 

This software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors, contributors, or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.

By using this tool, you acknowledge that you are loading third-party files onto your camera hardware. The creator of this repository is not responsible for any bricked devices, corrupted SD cards, lost photos, or unexpected behavior resulting from the use of generated filter files.
