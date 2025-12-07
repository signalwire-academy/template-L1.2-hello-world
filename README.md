# Lab 1.2: Hello World Agent

**Duration:** 45 minutes
**Module:** M1.2 - Your First Agent
**SDK Version:** signalwire-agents >= 1.0.11

## Objectives

By completing this lab, you will:

- Create a minimal working agent
- Configure basic prompt and voice
- Test with swaig-test CLI
- Understand generated SWML

## Prerequisites

- Completed Lab 1.1 (Environment Setup)
- Python 3.10+ installed
- Virtual environment activated

## Instructions

### 1. Set Up Your Environment

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Create Your Agent

Edit `solution/agent.py` to create a Hello World agent:

**Requirements:**
- [ ] Import `AgentBase` from `signalwire_agents`
- [ ] Create an agent instance with name "hello-agent"
- [ ] Add a prompt section with role "Role" and a friendly greeting message
- [ ] Add English language with voice "rime.spore"
- [ ] Run the agent in the main block

### 3. Test Your Agent

```bash
# Verify agent loads
swaig-test solution/agent.py --list-tools

# Check SWML output
swaig-test solution/agent.py --dump-swml
```

### 4. Submit

Push your changes to trigger auto-grading:

```bash
git add solution/agent.py
git commit -m "Complete L1.2 Hello World Agent"
git push
```

## Grading

Your submission is auto-graded on push. Check the Issues tab for results.

| Check | Points |
|-------|--------|
| Agent instantiates without errors | 25 |
| SWML is valid with sections.main | 25 |
| Prompt contains greeting message | 25 |
| Language configured as English | 25 |
| **Total** | **100** |

**Passing Score:** 70%

## Reference

See `reference/starter.py` for a boilerplate template.

## Help

- [SignalWire AI Agents Documentation](https://developer.signalwire.com/ai)
- [Module 1.2 Course Content](https://signalwire-academy.github.io/course-content/level-1/m1.2-first-agent/)

---

*SignalWire AI Agents Certification - Level 1*
