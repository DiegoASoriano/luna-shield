# Luna Shield

> "No queremos vigilar más. Queremos proteger mejor."

Luna Shield is a preventive digital assistant for teenagers aged 13-17 that detects risk situations in conversations in real time. It presents itself as a friendly animated avatar that accompanies the teenager in a non-threatening way, explaining risks and only escalating alerts to a guardian when necessary.

Built for **Hackathon 404: Threat Not Found** — U.S. Embassy in Mexico + StartupLab MX · April 24-26, 2026 · CDMX.

---

## The Problem

Over 13 million teenagers in Mexico have a smartphone with access to the internet and social media. The risks they face online — grooming, emotional manipulation, deceptive contact, and requests for personal data — are real and growing. Existing parental control tools like Qustodio, Bark, or Family Link talk to the parent, not the teenager. The teenager feels watched, uninstalls the app, and the risk persists.

---

## The Solution

Luna Shield puts the teenager at the center. When it detects a risk signal in a conversation, it:

1. Alerts the teenager first with empathetic, clear language.
2. Explains why the situation is dangerous.
3. Gives the teenager options: ignore, block, save evidence, or ask for help.
4. Only notifies the guardian if the risk level justifies it.

### Risk escalation system

| Level | What it detects | What Luna does | Notifies guardian |
|-------|----------------|----------------|-------------------|
| Low | Unusual language, basic personal questions | Soft message to teenager only | No |
| Medium | Data requests, moderate emotional pressure | Alert to teenager + general summary to guardian | Summary |
| High | Active grooming, threats, photo requests | Immediate alert to teenager + full detail to guardian | Immediately |

---

## Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------|
| Frontend | React + Tailwind + Lottie | Teenager and tutor interfaces |
| Backend | Python + FastAPI | API connecting all components |
| AI | Gemini API | Message classification and responses |
| Database | Supabase | Alerts and session storage |
| Animations | Lottie / CSS | Luna's animated states |
| Design | Figma | Wireframes and mockups |
| Deploy | Vercel + Railway | Frontend and backend hosting |

---

## AI Tools Used

<!-- 
  MAXIMILIANO — fill this section before the Sunday 12pm deadline.
  This section is MANDATORY. Missing it is grounds for disqualification.
  Format:
  - Tool name: what it was used for and to what extent.
-->

| Tool | Purpose | Extent of use |
|------|---------|---------------|
| Gemini API (Google) | Risk classifier for messages. Receives each message and returns risk level, category and explanatory response for the teenager. | 100% of detection logic |
| <!-- other AI tools used during the event --> | | |

---

## Project Structure
```
luna-shield/
├── frontend/        # React app — Adriana Solís
│   ├── src/
│   └── public/
├── backend/         # FastAPI + Supabase — Jesús Ortiz & Maximiliano Ayala
│   ├── routers/
│   └── models/
├── design/          # Wireframes, mockups, Lottie files — Ángel García
└── docs/            # Gemini prompt, test dataset, demo script — Maximiliano Ayala
```

## Running the Project Locally

<!-- JESÚS — fill this section before the Sunday 12pm deadline -->

### Prerequisites
<!-- list Python version, Node version, required accounts -->

### Backend
```bash
# instructions here
```

### Frontend
```bash
# instructions here
```

### Environment variables
<!-- explain what goes in .env files for both frontend and backend -->

---

## Links

- **Live demo:** <!-- Adriana — add Vercel URL -->
- **Demo video:** <!-- Diego — add YouTube or Google Drive link -->

---

## Validation

On Saturday April 25, the prototype was tested with real users:

<!-- 
  ADRIANA — fill this section after Saturday's validation session.
  Include: user profiles (no names), key findings, what changed in the prototype based on feedback.
-->

---

## Team

| Name | Role |
|------|------|
| Adriana Solís | Frontend, user validation |
| Ángel García | UX/UI, avatar design, animations |
| Diego Soriano | Pitch, strategy, project management |
| Jesús Ortiz | Backend, infrastructure |
| Maximiliano Ayala | AI, prompt engineering, risk classifier |


---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
