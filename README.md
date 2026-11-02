# EduCreator: Generative AI–Powered Smart Educational Content Creation Platform

**Major Project | Phase 1 External Review**
**Group ID:** CSDMP230035
**Guide:** Mr. Feroz Amer
**Company:** Manac Pvt. Ltd.

**Team**
- Mohammed Shanawaz Uddin (160923750082)
- Mir Junaid Ali Khan (160923750087)
- Mohd Syhoab (160923750078)

## Abstract

Teaching quality depends on well-prepared notes, slides, assessments and lab material, but preparing these manually takes hours and often results in inconsistent formats. Large language models can draft such content quickly, yet their free-form output is difficult to reuse, check or export. Existing tools are also isolated, offer limited personalisation, and provide few export options or analytics.

EduCreator is a web-based platform that uses the Google Gemini API together with JSON-schema validation to generate structured, consistent and exportable educational content. An educator selects a content type and provides a topic, grade level and difficulty, with an optional syllabus. The system fills a prompt template, attaches the target JSON schema and requests the output from Gemini. The response is validated for required fields and data types, and if validation fails Gemini is asked again, so only valid output reaches the educator. Validated content is previewed, saved to a content hub and project repository, and exported as PDF, DOCX, TXT or JSON.

The platform provides nine AI content generators: lecture notes, slide decks, quizzes and assessments, assignments, lab manuals, flashcards, a Bloom's-taxonomy question bank, and study guides with rubrics. It also includes an AI chat assistant, a content hub, project and document management, and an admin analytics dashboard for tracking users, generations and API usage. Access is controlled through authentication and role-based access control (RBAC) with three user roles. In total, 13 modules are integrated into one secured platform.

EduCreator is built with Django (Python) for the backend, the Google Gemini API for generation, JSON-schema validation for output control, and HTML, CSS and JavaScript templates for the frontend. Each generator follows a single pattern (form, prompt service, schema validator, rendered view), so a new content type needs only a new template and schema.

Planned future work includes retrieval-augmented generation (RAG) over syllabi, LMS integration (Moodle), multilingual output, student analytics, collaboration features, fact-checking quality checks, PPTX export, and a formal user study.

**Keywords:** Generative AI, Large Language Models, Google Gemini, JSON Schema, Educational Content Generation, Django, Role-Based Access Control
