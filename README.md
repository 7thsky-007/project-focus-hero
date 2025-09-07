# project-focus-hero
Building AI Course Project 
# Focus Hero — AI Study & Play Balance App

## Idea in a nutshell
**Focus Hero** is a kid-friendly mobile/web app that helps children balance study time, playtime, and screen entertainment using gentle AI personalization, fun challenges, and rewards. The app encourages healthy habits rather than harsh restrictions — it nudges kids toward breaks, offline play, and focused study sessions with playful characters and progress rewards.

---

## Background / Problem
Excessive and unmanaged screen time is linked to sleep problems, reduced attention, and negative mood in children. Parents often struggle to strike the right balance between learning, play, and screen entertainment. In smaller towns like Ambikapur, access to structured guidance and child-focused digital-wellness tools can be limited. As a product designer who cares about usable, humane tech, I want to build an approachable tool that helps kids form healthier routines.

**Personal motivation:** I want to create a product that is simple, respectful of family values, and effective for kids and parents alike.

---

## Target users & context
- **Primary users:** Children aged ~6–12 (with parental controls)
- **Secondary users:** Parents / caregivers who monitor and guide routines
- **Context:** Home use, after-school hours, weekends; suitable for low-bandwidth environments

---

## Core features
1. **Smart Schedule Builder**
   - AI suggests daily schedules balancing study, active play, and screen time based on child’s age, school hours, and parent preferences.

2. **Focus Sessions (Pomodoro-like)**
   - Timed study blocks with short breaks. AI adapts block length based on past engagement.

3. **Play & Break Suggestions**
   - Offers offline play ideas (simple games, drawing prompts, quick exercises) when a break is due.

4. **Fun Challenges & Rewards**
   - Gamified quests, collectible badges, and gentle progress streaks to motivate healthy habits.

5. **Personalized Nudges**
   - Friendly on-screen character gives context-aware prompts (e.g., “Time for fresh air!” or “Let’s do a 5-minute stretch”).

6. **Parent Dashboard**
   - Overview of daily balance, recommended adjustments, and an emergency override. Privacy-first reporting (no raw audio/images stored).

7. **Low-data Mode**
   - Works with minimal internet; most logic runs on-device.

---

## Data & AI techniques
- **Input data**
  - User-provided: child age, school schedule, preferred subjects, parental rules.
  - Interaction logs (time spent in sessions, completion of breaks/challenges) — stored locally or opt-in for cloud sync.
  - Optional: simple mood check-ins (emoji-based) to personalize suggestions.

- **AI techniques**
  - **Personalization rules + lightweight ML**: start with rule-based scheduling and augment with simple supervised learning (e.g., logistic regression or a small decision-tree model) to predict optimal focus/break durations based on past session success.
  - **Recommender logic**: recommend break activities and challenges using simple collaborative filtering or content-based matching.
  - **NLP (optional, minimal)**: if child types short responses, tiny intent detection for mood (happy, bored, tired) — keep models tiny and local.

- **Privacy-first approach**
  - Models run on-device where possible. Minimal data collection and transparent opt-in for cloud features.

---

## MVP (Minimum Viable Product) plan
1. **Phase 1 (MVP)** — Core features:
   - On-device schedule builder (rule-based)
   - Focus sessions timer + manual rewards
   - A small set (20–30) of offline play suggestions
   - Parent view with daily summary (no cloud)

2. **Phase 2** — Personalization:
   - Add local ML to adjust session lengths
   - Gamification improvements, badges, and streak logic

3. **Phase 3** — Scale & safety:
   - Optional encrypted cloud sync, multilingual support, partnerships with schools

---

## Evaluation metrics
- **Engagement**: percentage of scheduled focus sessions completed.
- **Balance score**: ratio of study : active play : entertainment time.
- **Retention**: daily/weekly active users (family level).
- **Satisfaction**: parent & child feedback surveys (emoji/quick ratings).
- **Wellness signals (opt-in)**: improvements in bedtime routines or reduced late-night screen usage.

---

## Challenges & Limitations
- **Behavioral change is hard**: app alone may not change habits without parental involvement.
- **Data quality & bias**: limited interaction data may make personalization noisy at first.
- **Age-appropriateness**: content must be carefully curated for different ages.
- **Privacy & safety**: must comply with child-data regulations; avoid collecting sensitive data.

---

## Ethical & privacy considerations
- Keep child safety front and center: no targeted advertising, minimal data retention, parental consent required for any cloud features.
- All sensitive processing (voice / mood inference) is opt-in and designed to run on-device.
- Provide clear disclosures and easy ways to delete data.

---

## Tech stack (suggested)
- **Frontend:** React Native (mobile) or Flutter (cross-platform) for simple deployment.
- **On-device ML:** TensorFlow Lite / Core ML / lightweight scikit-learn models compiled for mobile.
- **Backend (optional):** Firebase (auth + encrypted sync) — only if users opt in.
- **Storage:** Local SQLite / secure storage for settings and logs.
- **Design:** Tailored UI with friendly mascot, big icons, and minimal text for kids.

---

## Example user stories
- *As a parent, I want a recommended after-school routine so my child studies and still plays outside.*
- *As a child, I want to earn stickers when I finish my study sessions.*
- *As a parent, I want a quick daily summary so I can see if my child spent too much time on entertainment apps.*

---

## What next / Roadmap
- Prototype UI flows and test with 5–10 families for initial feedback.
- Add multilingual support (English + Hindi) and low-bandwidth mode.
- Partner with local schools or community centers for pilot testing.
- Expand features: guided relaxation exercises and school-subject micro-practice (optional).

---

## Acknowledgments & inspiration
- Idea inspired by concerns around kids’ screen time and mental wellness.
- Product design perspective shaped the UX focus on gentle nudges and gamification.
- Open-source tools and mobile ML libraries will be used for prototyping.

---

## Contact
**Author:** Arsh — 7arshsky@gmail.com 

