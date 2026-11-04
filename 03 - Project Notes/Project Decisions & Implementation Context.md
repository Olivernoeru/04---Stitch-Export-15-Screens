# Project Decisions & Implementation Context

**Project:** Ruang Aman  
**Document status:** Final project context for Ollama and Stitch  
**Updated:** 4 November 2026

## 1. Purpose of this file

This file provides the fixed project context that an AI assistant must follow when reading the knowledge base or supporting design implementation. It does not replace the six UX/UI documents in `02 - UX UI Documents` and must not be used to create new scope.

## 2. Source hierarchy

When information differs, follow this order:

1. Original assignment brief and source materials in `01 - Client Source`.
2. Confirmed project decisions recorded in this file and in the six final UX/UI documents.
3. Questionnaire data in the original CSV.
4. Supporting UX study cases and reference materials.

Do not treat unrelated examples inside source documents as requirements for Ruang Aman.

### Source-file caution

`01 - Client Source/04 - Tugas Kelompok UX/Tugas Kelompok 3 UX.md` contains the assignment instructions and also a separate example project named **Financial Guard**. Financial Guard is not Ruang Aman. Do not transfer its features, user flows, visual style, data, or requirements into this project. Use that file only for relevant assignment instructions and rubric context.

The UX Study Case files contain multiple research and competitor examples. Treat them as supporting references only. Do not copy unrelated product features or assumptions into Ruang Aman.

## 3. Fixed product identity and scope

- Product name: **Ruang Aman**.
- Platform: mobile application for Android and iOS.
- The application can be used without login or registration.
- The prototype scope is fixed at **15 screens**:
  1. Splash Screen
  2. Onboarding
  3. Masuk/Mulai
  4. Beranda
  5. Butuh Bantuan
  6. Pilih Jenis Kebutuhan
  7. Panduan Langkah Awal
  8. Checklist Panduan
  9. Cari Layanan
  10. Daftar Layanan
  11. Detail Layanan
  12. Informasi Bantuan Hukum
  13. Kenali Hakmu
  14. FAQ
  15. Profil & Pengaturan Privasi
- Peta Layanan is included as a map mode within screen 10 and a map action from screen 11. It is not an additional screen.
- Tersimpan is included as a collection within screen 15, with a shortcut on screen 4 and save actions on relevant content screens. It is not an additional screen.
- Do not add screens or features beyond this approved scope.

## 4. Fixed need categories

Screen 6 contains exactly four categories:

1. Bantuan Hukum (K1)
2. Pendampingan (K2)
3. Informasi Pelaporan (K3)
4. Bantuan Darurat (K4)

All four categories use the same main sequence from screen 6 through screen 7, screen 8, screen 9, screen 10, screen 11, and Hubungi Layanan. Their guide content and service filters differ by category. Quick Help on the home screen is a shortcut to Bantuan Darurat (K4), not a fifth category.

The product may be used by someone seeking help for themselves or by someone supporting a person close to them. Do not create a fifth category or a separate unapproved helper flow.

## 5. Fixed Quick Exit behavior

- Quick Exit is available from Onboarding, Masuk/Mulai, and all main application screens.
- When pressed, the application immediately switches to a neutral-looking page.
- No confirmation dialog appears before switching.
- The neutral page must look ordinary and must not show the Ruang Aman name, logo, brand colors, or sensitive application content.
- Quick Exit hides the application display. It does not delete checklist progress, saved items, or application settings.
- PIN is an optional additional security feature. If the user enables it, PIN is required before returning to the application content. If it is not enabled, the user can return without entering a PIN.
- Do not invent a specific gesture or hidden interaction for returning from the neutral page unless it is explicitly included in the approved UI design.
- The app-switcher preview must not reveal sensitive content, in line with the approved Quick Exit privacy requirement.

## 6. Research data and participants

### Questionnaire

- The CSV in `01 - Client Source/05 - Kuesioner` contains **20 complete responses**.
- All 20 rows contain answers to the core questionnaire questions.
- The six UX/UI documents use the 20 actual responses. Do not reduce the data to 10 or 18 respondents and do not fabricate or remove responses.
- The project stakeholder indicated that 10 respondents would be sufficient for the assignment, but the supplied dataset contains 20 complete responses. Use the actual dataset in the analysis.
- Findings are descriptive and must not be generalized to all victims or the wider population.

### Interviews and usability testing

The three designated participants are:

- Lili
- RA (Riska Amalia)
- Syifa

Two interview-based personas will be included separately in the presentation slides after interview notes are available. The `02 - User Persona` knowledge-base document contains questionnaire-based need archetypes and must not invent personal identities, ages, occupations, quotations, or experiences.

Usability-testing findings must only be written after actual testing has been conducted and results are available.

## 7. Content and data integrity

- The initial guide material is confirmed as available. Use the source material provided for guide content, checklist content, legal-aid information, and victim-rights information.
- Do not invent legal procedures, rights, contact details, service names, addresses, operating hours, costs, or map locations.
- The ZIP audited on 4 November 2026 did not contain a complete service directory with verified names, contacts, addresses, and locations. Until that data is supplied, service screens must show a clear unavailable-data state rather than dummy service records.
- The source materials must remain unchanged.

## 8. Language and document standards

- Use clear, natural, professional Indonesian.
- Do not use the terms “Klien”, “Client”, “Pihak Klien”, or similar wording in the final UX/UI documents.
- Avoid semicolons. Use periods, commas, colons, numbered lists, or bullet points as appropriate.
- Keep terms consistent across Research Analysis, User Persona, User Stories & Requirements, UX PRD, UI PRD, and User Flow/Flowchart/Customer Journey Map.
- Do not introduce new recommendations, optional features, unresolved questions, or scope changes.

## 9. Implementation handoff

The six final UX/UI documents are the primary specification for design implementation. Use them together rather than treating any single document as the only source of truth.

The next implementation stage uses Ollama for local model/context support and Stitch for interface design implementation. The design target remains the approved 15-screen Ruang Aman prototype. Keep implementation decisions traceable to the final documents and fixed project decisions above.
