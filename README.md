Excuse Evaluation Dataset (RLHF Annotation Simulation)

This project demonstrates rubric-based evaluation, scoring, and ranking of LLM-generated responses, simulating real-world AI training workflows.

Overview

This project simulates real-world AI data annotation and evaluation workflows, similar to those used in RLHF (Reinforcement Learning from Human Feedback).
The goal was to develop practical experience in:
	•	rubric-based evaluation
	•	comparative ranking
	•	identifying edge cases in natural language responses
The dataset consists of 20 tasks where multiple responses are evaluated using a structured rubric.

Task Description
Each task follows the prompt:
"Write an excuse for missing work today."
For each task:
	•	3 responses (A, B, C) are generated
	•	Each response is evaluated independently across 4 criteria
	•	A final ranking is assigned based on overall quality

Evaluation Criteria
Each response is scored from 1–5 on the following:
	•	Believability — How realistic and convincing the excuse is
	•	Specificity — Level of detail and contextual clarity
	•	Emotional Plausibility — Whether the tone feels natural and human
	•	Suspicion (reversed) — Likelihood of raising doubt (higher = less suspicious)
All criteria use:
1 = poor, 5 = excellent

Methodology
	•	Responses were scored independently before ranking
	•	Ties in scoring were resolved at the ranking stage (scores were not adjusted)
	•	Evaluation avoided assumption bias by focusing on plausibility rather than ideal behavior
	•	Emphasis was placed on consistency across tasks

Key Learnings
	•	Distinguishing between weak vs unrealistic responses is critical
	•	Overly detailed responses can increase suspicion
	•	Real-world plausibility is more important than logical perfection
	•	Consistent scoring is more valuable than perfect scoring

Files
	•	dataset.csv — annotated dataset
	•	rubric.md — detailed evaluation rubric

Purpose
This project is intended to demonstrate readiness for roles such as:
	•	AI Data Annotator
	•	AI Trainer / Evaluator
	•	RLHF / Model Evaluation Contributor

Key Skills Demonstrated
- Rubric design and refinement
- Consistent multi-criteria evaluation
- Comparative ranking of model outputs
- Edge-case analysis and bias mitigation
- Structured dataset creation for AI training

Author
Jerard Venter Cape Town, South Africa
