# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an educational project focused on creating AI curriculum documentation in Czech language. The repository contains course materials for a comprehensive 60-hour AI fundamentals course.

## Project Structure

```
.
├── hourList.md                  # 60-hour AI curriculum outline in Czech
├── source.txt                   # Reference documentation links for AI/ML tools
├── AI_Zaklady_Hodina_01.ipynb   # Jupyter notebook for Hour 1: Introduction to AI
├── AI_Zaklady_Hodina_02.ipynb   # Jupyter notebook for Hour 2: History of AI
├── AI_Zaklady_Hodina_03.ipynb   # Jupyter notebook for Hour 3: Future of AI
├── AI_Zaklady_Hodina_04.ipynb   # Jupyter notebook for Hour 4: Related fields
├── AI_Zaklady_Hodina_05.ipynb   # Jupyter notebook for Hour 5: Human vs Machine Intelligence
├── AI_Zaklady_Hodina_06.ipynb   # Jupyter notebook for Hour 6
├── AI_Zaklady_Hodina_07.ipynb   # Jupyter notebook for Hour 7
├── AI_Zaklady_Hodina_08.ipynb   # Jupyter notebook for Hour 8
├── AI_Zaklady_Hodina_09.ipynb   # Jupyter notebook for Hour 9
├── AI_Zaklady_Hodina_10.ipynb   # Jupyter notebook for Hour 10
├── AI_Zaklady_Hodina_11.ipynb   # Jupyter notebook for Hour 11
├── AI_Zaklady_Hodina_12.ipynb   # Jupyter notebook for Hour 12
├── AI_Zaklady_Hodina_13.ipynb   # Jupyter notebook for Hour 13
├── AI_Zaklady_Hodina_14.ipynb   # Jupyter notebook for Hour 14
├── AI_Zaklady_Hodina_15.ipynb   # Jupyter notebook for Hour 15
├── AI_Zaklady_Hodiny_16_17.ipynb # Jupyter notebook for Hours 16-17
├── AI_Zaklady_Hodiny_18_20.ipynb # Jupyter notebook for Hours 18-20
└── CLAUDE.md                    # This file
```

## Key Information

### Purpose
This is a documentation repository for AI educational content, not a software development project. The materials are designed to teach AI fundamentals in Czech.

### Course Content Areas
The curriculum (hourList.md) covers:
- Introduction to AI (Hours 1-10)
- AI algorithms and problem-solving (Hours 11-20)
- Decision-making and probability (Hours 21-30)
- Machine learning (Hours 31-40)
- Neural networks (Hours 41-54)
- AI ethics and future (Hours 55-60)

### Resource Links
The source.txt file contains documentation links for common AI/ML tools and frameworks:
- Jupyter Notebook and Google Colab
- Data science libraries: NumPy, Pandas, Matplotlib, Seaborn
- Machine learning frameworks: Scikit-learn, TensorFlow
- Ollama

## Working with Jupyter Notebooks

The course materials are primarily delivered through Jupyter notebooks (.ipynb files). Each notebook corresponds to specific hours in the curriculum:
- Individual hour notebooks: `AI_Zaklady_Hodina_XX.ipynb`
- Multi-hour notebooks: `AI_Zaklady_Hodiny_XX_YY.ipynb`

### Notebook Structure
Each notebook typically contains:
- Theoretical explanations in Markdown cells
- Practical Python code examples
- Interactive exercises for students
- Homework assignments

## Development Guidelines

Since this is a documentation project:
- Focus on maintaining clear, educational content in Czech
- Preserve the structured format of the curriculum
- When updating content, ensure consistency with the established 60-hour format
- Keep resource links in source.txt up to date
- Maintain consistency between hourList.md and the corresponding Jupyter notebooks

## Technical Stack

The course uses the following Python libraries and tools:
- **Environment**: Google Colab / Jupyter Notebooks
- **Core Libraries**: NumPy, Pandas, Matplotlib, Seaborn
- **ML Frameworks**: Scikit-learn, TensorFlow
- **LLM Tools**: Ollama (for local language model experiments)
- **Other**: transformers library (for GPT models)

## Notes

- No build, test, or deployment processes are currently defined
- The project is designed to be run in Google Colab or Jupyter environments
- Currently covers hours 1-20 with notebooks (hours 21-60 may need to be created)

## Detailed Notebook Descriptions

### AI_Zaklady_Hodina_01.ipynb - Introduction to AI
**Content Overview:**
- Definition of artificial intelligence and its various types (weak vs. strong AI)
- Historical context and modern relevance
- Introduction to Python programming with Google Colab
- Basic neural network concepts using PyTorch

**Code Style:**
- Clean, well-commented code with Czech explanations
- Progressive complexity from print statements to neural networks
- Interactive visualizations using matplotlib
- Hands-on exercises with immediate feedback

**Pedagogical Approach:**
- Starts with relatable examples (calculator vs. AI)
- Combines theory with practical implementation
- Uses visual aids (diagrams, plots) to explain abstract concepts
- Includes homework assignments for reinforcement
- Gradio interface for interactive experimentation

**Key Technologies:** PyTorch, NumPy, Matplotlib, Gradio

---

### AI_Zaklady_Hodina_02.ipynb - History of AI
**Content Overview:**
- Timeline of AI development from 1943 to present
- Key personalities and their contributions
- Evolution of AI approaches (symbolism vs. connectionism)
- Turing test and its implications

**Code Style:**
- Extensive use of data visualization for historical timelines
- Interactive network graphs showing relationships between concepts
- Clean separation of theory and practical examples

**Pedagogical Approach:**
- Chronological narrative structure
- Visual timeline representations
- Interactive quizzes to test understanding
- Practical implementation of historical algorithms

**Key Technologies:** NetworkX, Matplotlib, Pandas, ipywidgets

---

### AI_Zaklady_Hodina_03.ipynb - Future of AI
**Content Overview:**
- Exploration of AGI and superintelligence concepts
- Societal impacts across various sectors
- Introduction to generative AI and language models
- Practical work with Ollama for local LLM deployment

**Code Style:**
- Integration with external APIs (Ollama)
- Asynchronous programming patterns
- Error handling for model interactions
- Clean abstraction of complex concepts

**Pedagogical Approach:**
- Scenario-based learning
- Hands-on experimentation with LLMs
- Discussion prompts for ethical considerations
- Real-world application examples

**Key Technologies:** Ollama, Transformers, Gradio, asyncio

---

### AI_Zaklady_Hodina_04.ipynb - Related Fields
**Content Overview:**
- Comparison of AI with data science, statistics, and traditional programming
- Cognitive science and philosophy connections
- Practical differences in problem-solving approaches
- Data preprocessing fundamentals

**Code Style:**
- Comparative code examples showing different approaches
- Well-structured data processing pipelines
- Clear separation of concerns in code organization

**Pedagogical Approach:**
- Comparative analysis methodology
- Practical exercises contrasting different approaches
- Visual representations of field relationships
- Group discussion activities

**Key Technologies:** Scikit-learn, Pandas, NumPy, Seaborn

---

### AI_Zaklady_Hodina_05.ipynb - Human vs Machine Intelligence
**Content Overview:**
- Comparative analysis of cognitive processes
- Strengths and limitations of each type of intelligence
- Practical demonstrations using GPT-2
- Pattern recognition exercises

**Code Style:**
- Clean implementation of transformer models
- Comparative algorithm implementations
- Performance benchmarking code
- Interactive comparison tools

**Pedagogical Approach:**
- Side-by-side comparisons
- Interactive challenges for students
- Performance metrics visualization
- Reflective exercises on intelligence types

**Key Technologies:** Transformers (GPT-2), TensorFlow, Plotly, Gradio

---

### AI_Zaklady_Hodina_06.ipynb - Ethics and Philosophy of AI
**Content Overview:**
- Bias in data and algorithms
- Philosophical questions about consciousness and free will
- Ethical guidelines and frameworks
- Practical bias detection and mitigation

**Code Style:**
- Implementation of bias detection algorithms
- Statistical analysis of fairness metrics
- Clear documentation of ethical considerations
- Reproducible analysis pipelines

**Pedagogical Approach:**
- Case study methodology
- Interactive bias exploration
- Group discussions on ethical dilemmas
- Practical exercises in fairness assessment

**Key Technologies:** Pandas, Scikit-learn, Matplotlib, Seaborn

---

### AI_Zaklady_Hodina_07.ipynb - AI in Everyday Life
**Content Overview:**
- Practical applications across industries
- Recommendation systems implementation
- Voice assistants and NLP basics
- Real-world data analysis

**Code Style:**
- Production-ready code examples
- API integration patterns
- Data pipeline implementations
- Clean visualization code

**Pedagogical Approach:**
- Real-world case studies
- Hands-on implementation of common AI applications
- Industry data analysis
- Interactive demonstrations

**Key Technologies:** TensorFlow, Pandas, Plotly, Speech Recognition libraries

---

### AI_Zaklady_Hodina_08.ipynb - AI in Games
**Content Overview:**
- Game AI algorithms (minimax, alpha-beta pruning)
- Reinforcement learning basics
- Implementation of game-playing agents
- Modern game AI techniques

**Code Style:**
- Object-oriented game implementations
- Efficient algorithm implementations
- Clear separation of game logic and AI
- Performance-optimized code

**Pedagogical Approach:**
- Learning through game development
- Progressive complexity in game AI
- Interactive game playing against AI
- Algorithm visualization

**Key Technologies:** NumPy, Matplotlib, Custom game engines, RL libraries

---

### AI_Zaklady_Hodina_09.ipynb - Mini Project
**Content Overview:**
- Project planning and problem definition
- Tool selection and prototyping
- Gradio interface development
- Complete AI application development

**Code Style:**
- Modular project structure
- Clean API design
- Comprehensive error handling
- User-friendly interface code

**Pedagogical Approach:**
- Project-based learning
- Peer collaboration encouragement
- Iterative development process
- Presentation skills development

**Key Technologies:** Gradio, Transformers, Ollama, Full-stack integration

---

### AI_Zaklady_Hodina_10.ipynb - Summary and Review
**Content Overview:**
- Comprehensive review of concepts
- Interactive knowledge testing
- Integration of all previous topics
- Preview of advanced topics

**Code Style:**
- Review exercises combining multiple concepts
- Clean, educational code examples
- Interactive quiz implementations
- Consolidated learning examples

**Pedagogical Approach:**
- Active recall methodology
- Peer teaching opportunities
- Comprehensive assessment
- Forward-looking connections

**Key Technologies:** All previously used libraries, Interactive widgets

---

### AI_Zaklady_Hodina_11.ipynb - State Space
**Content Overview:**
- State space representation and modeling
- Graph theory applications in AI
- Problem formulation techniques
- Neural network integration with search algorithms

**Code Style:**
- Graph data structure implementations
- Visualization-heavy code
- Clean abstraction of state space concepts
- Efficient search implementations

**Pedagogical Approach:**
- Visual learning through graph representations
- Step-by-step problem modeling
- Interactive state space exploration
- Practical problem-solving exercises

**Key Technologies:** NetworkX, Matplotlib, PyTorch, Custom visualization tools

---

### AI_Zaklady_Hodina_12.ipynb - Search Algorithms Part 1
**Content Overview:**
- Breadth-First Search (BFS) implementation
- Depth-First Search (DFS) implementation
- Algorithm comparison and complexity analysis
- Practical applications in pathfinding

**Code Style:**
- Clean algorithm implementations with Czech comments
- Efficient use of data structures (deque, stack)
- Comprehensive visualization of search processes
- Performance benchmarking code

**Pedagogical Approach:**
- Algorithm visualization for understanding
- Comparative analysis methodology
- Hands-on implementation exercises
- Real-world problem applications

**Key Technologies:** Collections, Matplotlib, NetworkX, Custom animations

---

### AI_Zaklady_Hodina_13.ipynb - Search Algorithms Part 2
**Content Overview:**
- Advanced search algorithms (A*, IDA*)
- Heuristic function design
- Optimization techniques
- Neural network-enhanced search

**Code Style:**
- Sophisticated algorithm implementations
- Priority queue optimizations
- Clean heuristic function designs
- Integration of ML with classical algorithms

**Pedagogical Approach:**
- Building on previous knowledge
- Practical heuristic development
- Performance analysis and optimization
- Hybrid AI approach demonstration

**Key Technologies:** heapq, NumPy, PyTorch, Scikit-learn

---

### AI_Zaklady_Hodina_14.ipynb - Constraint Satisfaction Problems
**Content Overview:**
- CSP theory and formulation
- Backtracking algorithms with neural heuristics
- Practical solvers (Sudoku, N-Queens)
- Transformer models for CSP

**Code Style:**
- Elegant CSP solver implementations
- Neural network integration patterns
- Clean constraint representation
- Efficient backtracking implementations

**Pedagogical Approach:**
- Problem-solving methodology
- Visual constraint representation
- Interactive puzzle solving
- Modern AI techniques application

**Key Technologies:** OR-Tools, Transformers, PyTorch, Gradio

---

### AI_Zaklady_Hodiny_16_17.ipynb - Maze and AI (Combined Hours)
**Content Overview:**
- Comprehensive maze generation and solving
- Multiple algorithm implementations
- Visual pathfinding demonstrations
- Performance comparisons

**Code Style:**
- Modular maze generation code
- Multiple solver implementations
- Rich visualization capabilities
- Benchmarking framework

**Pedagogical Approach:**
- Extended project-based learning
- Algorithm comparison methodology
- Visual learning through animations
- Comprehensive skill integration

**Key Technologies:** Pygame, Matplotlib, Custom visualization, Multiple search algorithms

---

### AI_Zaklady_Hodiny_18_20.ipynb - Extended Project (Combined Hours)
**Content Overview:**
- Complete AI system development
- Integration of multiple concepts
- Advanced problem-solving applications
- Production-ready implementations

**Code Style:**
- Professional project structure
- Comprehensive documentation
- Error handling and logging
- Performance optimization

**Pedagogical Approach:**
- Capstone project methodology
- Independent problem-solving
- Peer review and collaboration
- Presentation and communication skills

**Key Technologies:** Full stack of previously learned tools, Custom integrations

---

## Teaching Methodology Summary

The course employs a consistent pedagogical approach across all notebooks:

1. **Progressive Complexity**: Each lesson builds upon previous knowledge, starting from basic concepts and advancing to complex implementations.

2. **Theory-Practice Balance**: Every theoretical concept is immediately followed by practical implementation, ensuring students understand both the "what" and the "how".

3. **Visual Learning**: Extensive use of visualizations (matplotlib, plotly, networkx) helps students grasp abstract concepts through visual representation.

4. **Interactive Engagement**: Gradio interfaces and interactive widgets allow students to experiment with AI models in real-time.

5. **Local Deployment Focus**: Integration with Ollama enables students to run AI models locally, understanding deployment considerations.

6. **Project-Based Learning**: Regular mini-projects and exercises reinforce learning through practical application.

7. **Modern Tools Integration**: Students learn industry-standard tools (PyTorch, TensorFlow, Transformers) preparing them for real-world applications.

8. **Ethical Considerations**: Ethics and bias are woven throughout the curriculum, not just isolated to specific lessons.

## Practical Applications for Workers

The curriculum is designed with practical workplace applications in mind:

- **Automation Skills**: Students learn to automate repetitive tasks using AI
- **Data Analysis**: Comprehensive pandas and visualization skills for data-driven decisions
- **Problem-Solving**: Systematic approach to breaking down complex problems
- **Tool Proficiency**: Hands-on experience with industry-standard AI/ML tools
- **Ethical Awareness**: Understanding of AI limitations and ethical considerations
- **Communication**: Practice explaining AI concepts to non-technical stakeholders through presentations