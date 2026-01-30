# MyBodyShape - AdSense Approval Project Blueprint

## 1. Project Overview

**Goal:** To modify the `mybodyshape.pages.dev` website to meet Google AdSense program policies and achieve approval for monetization.

**Core Problem:** The website, while functional, suffers from "thin content" and lacks the markers of trust, authority, and comprehensiveness that AdSense requires. The main issues are insufficient static content, underdeveloped policy pages (`about`, `contact`, `privacy`), and a lack of a Terms of Service page.

**Strategy:** The project will focus on transforming the site from a simple single-page tool into a content-rich, authoritative resource for body shape analysis and fashion. This involves a significant expansion of written content and a professionalization of all informational and policy pages.

---

## 2. Implemented Features & Design (as of Initial State)

### Core Functionality
- **AI Body Shape Analysis:** Users can upload a full-body photo to receive an analysis of their body type.
- **Client-Side Processing:** Image analysis is performed in the browser using TensorFlow.js and a Teachable Machine model. No user photos are uploaded to a server.
- **Interactive Survey:** A short questionnaire complements the AI analysis to refine the results.
- **Result Display:** A dedicated result page shows the user's body type, a description, styling tips, and representative celebrities.
- **Language Support:** The UI supports both Korean and English.

### Design & UX
- **Visual Style:** Clean, modern, and mobile-first design with a pink and gray color scheme.
- **Layout:** Single-column layout centered on the page.
- **Navigation:** Simple header and footer navigation linking to `index`, `about`, `contact`, and `privacy` pages.

### Pages
- **`index.html`:** The main application page containing the upload tool and dynamically displayed views (loading, survey, result). Includes a brief intro to the service.
- **`about.html`:** A short, personal story from the creator.
- **`contact.html`:** A page with a single email address for contact.
- **`privacy.html`:** A brief policy stating that no data is stored and images are processed client-side.

---

## 3. Current Task: AdSense Compliance Enhancement

This section outlines the plan for the currently requested changes.

### Phase 1: Content & Policy Overhaul

#### 1. **Enhance `index.html`**
   - **Objective:** To add substantial, high-quality, static content to make the main page a valuable resource in itself.
   - **Changes:**
     - **Remove External Links:** Delete the two links to the Naver blog to keep users on the site.
     - **Remove Anti-UX Script:** Remove the `contextmenu` event listener that blocks right-clicking.
     - **Add Detailed Body Type Sections:**
       - Create three distinct, comprehensive sections for **Straight, Wave, and Natural** types.
       - Each section will include:
         - A detailed, non-generic description of the body type's characteristics.
         - In-depth styling advice (Dos and Don'ts).
         - A list of recommended clothing items and fabrics.
         - Examples of celebrity styles for inspiration.
     - **Add FAQ Section:**
       - Create a Frequently Asked Questions area to address common user queries about the technology, accuracy, privacy, and styling.

#### 2. **Rewrite `privacy.html`**
   - **Objective:** To replace the simple policy with a comprehensive, professional, and trustworthy document.
   - **Changes:**
     - Draft a new policy including clauses on: Data Controller, Types of Data Collected (Google Analytics, AdSense cookies), Purpose of Processing, User Rights (GDPR/CCPA-inspired), Children's Privacy, and contact details for the data controller.

#### 3. **Rewrite `about.html`**
   - **Objective:** To build authority and trust.
   - **Changes:**
     - Restructure the page to include:
       - **Our Mission:** A clear statement of the site's goals.
       - **Our Technology:** An accessible explanation of the AI technology used.
       - **Our Team:** A more professional presentation of the creator(s).
       - **Our Commitment:** A statement on user privacy and data ethics.

#### 4. **Rewrite `contact.html`**
   - **Objective:** To appear more professional and organized.
   - **Changes:**
     - Create a structured page with different contact categories (e.g., General Inquiry, Technical Issue) to guide users, even if they lead to the same email address.
     - Add information about expected response times.

#### 5. **Create `tos.html` (Terms of Service)**
   - **Objective:** To add a critical legal page required for most online services.
   - **Changes:**
     - Draft a standard Terms of Service document covering user responsibilities, intellectual property, disclaimers, and limitations of liability.

#### 6. **Update Footer**
   - **Objective:** To ensure all legal and informational pages are accessible.
   - **Changes:**
     - Add a link to the new `tos.html` page in the footer of all relevant pages.

#### 7. **Verify AI Model Files**
   - **Objective:** To ensure the core functionality of the site is not broken.
   - **Changes:**
     - List the project files to check for the presence of the `my_model` directory and its contents (`model.json`, `metadata.json`). Report findings to the user.
