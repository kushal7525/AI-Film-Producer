
# AI Movie Production Agent  
*A smart single-agent assistant for film production planning, powered by LLMs and streamlined workflow logic*

## 🎬 What is this?  
The **AI Movie Production Agent** is an open-source tool built to assist creators in planning, structuring and managing movie production workflows. This single-agent application handles script inputs, production scheduling, resource allocation, budget breakdowns and other film-centric planning tasks—enabling filmmakers, producers or developers to prototype and iterate on film-project workflows using a modern LLM-driven interface.

## ✅ Key Features  
- **Script & concept analysis** – Submit a film concept or script segment; the agent will identify key scenes, characters, assets and production tasks.  
- **Production scheduling** – Generate a schedule with phases (pre-production, production, post-production), milestones and dependencies.  
- **Budget breakdown** – Produce a budget estimate by category (cast, crew, equipment, locations, VFX) and highlight cost-saving opportunities.  
- **Resource & role checklist** – Create a checklist of required personnel, equipment, locations and logistics.  
- **Task-execution suggestions** – Get actionable next-steps to move your film project forward: e.g., “lock location by this date”, “hire sound mixer”, “allocate contingency fund”.

## 🧠 Why it matters  
Film production projects are inherently complex, involving many moving parts and coordination across domains. This agent reduces friction by:  
- Providing a single unified interface for planning, scheduling and budgeting  
- Using LLM intelligence to interpret high-level creative input (script, synopsis) and generate structured outputs  
- Offering a developer-friendly template for extending or customizing film-production workflows  
- Serving as a rapid prototyping sandbox for indie filmmakers, production startups or film-tech innovators

## 🛠 Getting Started  
### Prerequisites  
- Python 3.10 or newer  
- Access to an LLM API (e.g., OpenAI, Gemini) with an API key  
- Basic familiarity with Python virtual environments

### Installation & Setup  
```bash
git clone https://github.com/kushal7525/AI-Film-Producer.git
cd AI-Film-Producer

python -m venv venv  
# On Windows:
venv\Scripts\activate  
# On macOS/Linux:
source venv/bin/activate

pip install -r requirements.txt
````

Create a `.env` file in the project root:

```env
LLM_API_KEY=your_api_key_here  
# (or whichever environment variable the app expects)
```

### Running the Agent

```bash
python movie_production_agent.py
```

Follow command-line prompts (or UI if provided) to input your film concept, script or initial data. The agent then produces structured outputs you can view/export.

## 📄 Input & Output Formats

### Input Example

Provide a film concept or script excerpt, for example:

```
Title: “Dreamscape”
Genre: Sci-fi Thriller
Logline: A neuroscientist explores dreams to save a comatose partner.
Key Scenes: inception, dream-levels, confrontation, awakening.
```

### Output Example

* Scene breakdown with scene durations
* Production schedule (dates, tasks, dependencies)
* Budget category list (with estimates)
* Resource checklist (crew roles, equipment, locations)
* Next-step action list (e.g., “Finalize storyboard by [date]”, “Secure location A by [date]”)

## 📈 Architecture & Workflow

1. **User input** — concept, script excerpt or production requirement.
2. **Agent execution** — A single-agent workflow uses an LLM prompt orchestration to parse input and generate multiple structured modules: scene analysis, schedule, budget, resources, actions.
3. **Output assembly** — The agent aggregates module outputs into a cohesive plan.
4. **User review & iteration** — User reviews outputs, optionally modifies input and re-runs for refinements.

## 🛠 Extending & Customising

* Swap in your preferred LLM / adjust prompts for tone, style or region-specific production contexts.
* Add new modules: e.g., **Marketing & Distribution Agent**, **VFX Scheduling Agent**, or **Casting Agent**.
* Integrate with production tools: e.g., export to project-management software (Trello, Asana), budget-tracking spreadsheets, storyboarding tools.
* Support multi-user collaboration / extend UI to a web or mobile front-end.

## ⚠️ Disclaimer

This tool is for **educational and planning purposes only**. It does *not* guarantee production-ready budgets, schedules or legal/financial advice. Always consult professional film-production services and legal counsel for real projects.

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch (e.g., `feature/new-module`)
3. Commit your changes and open a pull request
4. Discuss and refine via issues or PR comments

## 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

## ⭐ Acknowledgments

* The open-source ecosystem
* LLM providers enabling creative workflows
* Inspiration from film-tech innovation communities

---

