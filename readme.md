# ArchiveNext

ArchiveNext is a React Native Android app built with Expo, offering a seamless solution for creating, previewing, scanning, and managing document templates such as birth certificates, death certificates, and marriage certificates. With the power of **Google ML Kit** for scanning and document digitization, the app delivers a high-quality user experience for digitizing physical documents, enabling better efficiency and accuracy.

---

## Demo Video

A video demonstration of the app's features is available below:

[![Watch the video](https://via.placeholder.com/728x90.png?text=Click+to+Watch+the+Demo)](YOUR_VIDEO_LINK_HERE)  
(*Replace `YOUR_VIDEO_LINK_HERE` with the actual link to your video.*)

---

## App Screenshots

### Home Screen  
The **Home Screen** serves as the starting point of the app. From here, users can navigate to various features like creating templates, scanning documents, and viewing saved templates. The design is intuitive, ensuring easy access to core functionalities.

![Home Screen](images/first.jpeg)

---

### Create Template Screen  
This screen allows users to create templates for certificates such as birth, death, or marriage.  

![Create Template Screen]()  
(*Replace with the actual screenshot of the Create Template Screen.*)

---

### Existing Templates Screen  
This screen displays all previously created templates. Users can select and edit templates or view their details.  

![Existing Templates Screen](https://via.placeholder.com/400x800.png?text=Existing+Templates+Screen)  
(*Replace with the actual screenshot of the Existing Templates Screen.*)

---

### Document Save Screen (Before and After Sync)  
- **Before Sync**: View unsynced documents that are stored locally.  
- **After Sync**: Documents synced successfully with the server or cloud storage.  

**Before Sync**  
![Document Save Before Sync](https://via.placeholder.com/400x800.png?text=Document+Save+Before+Sync)  
(*Replace with the actual screenshot showing documents before sync.*)  

**After Sync**  
![Document Save After Sync](https://via.placeholder.com/400x800.png?text=Document+Save+After+Sync)  
(*Replace with the actual screenshot showing documents after sync.*)

---

## Features

### Core Functionalities
- **Template Management**:  
  - Create templates for certificates (birth, death, marriage).
  - Preview and save templates for future use.
  
- **Document Scanning with ML Kit**:  
  - High-quality and consistent document digitization with advanced edge detection.
  - Automatic cropping, rotation, and shadow/stain removal.
  - On-device processing to preserve user privacy.

- **Saved Document Viewer**:  
  - Browse, view, and organize saved templates and digitized documents.
  - Open documents in an integrated PDF Viewer.

- **Intuitive User Experience**:  
  - Built with React Navigation for smooth app navigation.
  - Lightweight Expo setup for quick deployment and prototyping.

### ML Kit Integration
Using ML Kit's Document Scanner API, the app provides:
- Automatic document detection and capture.
- Editing capabilities (cropping, filters, shadow removal, etc.).
- Privacy-focused, on-device processing without needing camera permissions.
- Low binary size impact by leveraging Google Play services.

---

## App Structure

The project is structured for scalability and maintainability:

```
src/
├── assets
│   ├── logo.png
│   └── michel_logo.png
├── components
│   ├── AppFooter.js
│   ├── CustomFormComponents.js
│   ├── Header.js
│   └── SectionHeader.js
├── screens
│   ├── BirthCertificateForm.js
│   ├── CreateTemplateScreen.js
│   ├── DeathCertificateForm.js
│   ├── ExistingTemplatesScreen.js
│   ├── HomeScreen.js
│   ├── MarriageCertificateForm.js
│   ├── PDFViewerScreen.js
│   ├── PreviewBirthCertificateScreen.js
│   ├── ScanScreen.js
│   ├── TemplateSuccessScreen.js
│   ├── ViewCertificateScreen.js
│   └── ViewSavedDocumentsScreen.js
└── utils
    ├── fileManager.js
    ├── firebase
    │   ├── config.js
    │   └── firebaseService.js
    ├── storage
    │   ├── certificateStorage.js
    │   └── index.js
    └── sync
        └── syncService.js
```

---

## Installation

Follow these steps to set up the app locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ArchiveNext.git
   cd ArchiveNext
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Install Expo CLI globally if not already installed:
   ```bash
   npm install -g expo-cli
   ```

4. Set up Firebase configuration in `src/utils/firebase/config.js`.

5. Start the development server:
   ```bash
   expo start
   ```

6. Run the app:
   - On an Android Emulator or connected device:
     ```bash
     expo run:android
     ```
   - Or via the Expo Go app by scanning the QR code from the terminal.

---

## Usage

### ML Kit Document Scanner API
- **Scanner Modes**: Choose between `SCANNER_MODE_BASE`, `SCANNER_MODE_BASE_WITH_FILTER`, or `SCANNER_MODE_FULL` for editing and cleaning capabilities.
- **Customizations**:  
  - Limit the number of pages scanned.  
  - Enable or disable gallery import.  

### Supported Actions
- Create templates for certificates.
- Scan physical documents and digitize them with advanced filters.
- View saved templates and export them as PDF files.

---


## Author

**Your Name**  
*Optional: Include links to your GitHub, LinkedIn, or other contact info.*

