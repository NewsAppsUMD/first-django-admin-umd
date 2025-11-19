# Interactive Django Admin Tutorial

An **interactive**, hands-on tutorial for building a Django admin interface, designed to be completed with AI assistance (Claude Code or GitHub Copilot). This tutorial teaches Django fundamentals through guided discovery and Socratic questioning.

## 🎯 What You'll Build

A custom Django administration panel for managing Academy Award invitee data—the same dataset used by the LA Times in their Oscar diversity reporting. You'll learn to:

- Design database tables using Django's ORM
- Load data from CSV files
- Create an intuitive admin interface
- Manage user permissions
- Export edited data

## 🤖 Interactive Learning Experience

This isn't a traditional "copy and paste" tutorial. Instead, you'll:

- **Make design decisions** and discuss trade-offs
- **Predict outcomes** before running commands
- **Explain concepts** in your own words
- **Reflect on learning** at key milestones

Your AI assistant (Claude or Copilot) will guide you through Socratic questioning, encouraging deeper understanding rather than just completing tasks.

## 📋 Prerequisites

Before starting, ensure you have:

1. **Command-line interface** (Terminal on Mac/Linux, Command Prompt on Windows)
2. **Text editor** (VS Code recommended)
3. **Python 3.9+** ([download here](https://www.python.org/downloads/))
4. **pipenv** ([installation instructions](https://pipenv.pypa.io/en/latest/install/))
5. **Git** and a GitHub account

## 🚀 Getting Started

### Option 1: GitHub Codespaces (Recommended for Beginners)

1. Fork this repository to your GitHub account
2. Click the **Code** button → **Codespaces** → **Create codespace on main**
3. Wait for the environment to load (includes VS Code in your browser!)
4. Install the **GitHub Copilot** or **Claude** extension
5. Open `docs/index.rst` and start following the tutorial

### Option 2: Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/NewsAppsUMD/first-django-admin-umd.git
   cd first-django-admin-umd
   ```

2. Install VS Code with either:
   - [GitHub Copilot extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)
   - [Claude Code extension](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code)

3. Open the project in VS Code:
   ```bash
   code .
   ```

4. Open `docs/index.rst` to begin the tutorial

## 📖 How to Use This Tutorial

### The Claude.md File

The `Claude.md` file contains instructions for your AI assistant on how to guide you through the tutorial. It establishes:

- **Socratic teaching approach**: Questions before answers
- **Encouraging tone**: Celebrating progress and normalizing mistakes
- **Active learning**: Prompts for prediction, experimentation, and reflection
- **Understanding checks**: Regular comprehension assessments

### Working with Your AI Assistant

As you progress through the tutorial, your AI assistant will:

1. **Ask you questions** before providing code or explanations
2. **Encourage you to predict** what will happen before running commands
3. **Check your understanding** by having you explain concepts
4. **Guide you through decisions** rather than making them for you
5. **Help you learn from errors** by asking diagnostic questions

### Example Interaction

```
📖 You: I'm ready to start Act 2: Hello Models

🤖 Assistant: Great! Before we create our first model, let's think about
data design. Look at the academy_invites_2014.csv file. What fields do
you see? What patterns do you notice about the "Branch" field?

📖 You: I see Name and Branch. Branch has values like "Actor", "Director"...

🤖 Assistant: Excellent observation! Now here's a design question: Should
we let users type anything for the Branch field, or restrict it to specific
choices? What are the pros and cons of each approach?

📖 You: Hmm, if we restrict it, data will be cleaner... but what if there's
a new branch type?

🤖 Assistant: You're thinking like a developer! Let's discuss that trade-off...
```

## 🗂️ Tutorial Structure

The tutorial is organized into 6 acts:

1. **Act 1: Hello Django** - Project setup & SQLite database initialization
2. **Act 2: Hello Models** - Database schema design with Django ORM
3. **Act 3: Hello Loader** - CSV import with custom management commands
4. **Act 4: Hello Admin** - Configuring Django's admin interface
5. **Act 5: Hello Newsroom** - Multi-user setup and permissions
6. **Act 6: Hello Homework** - Model migrations and schema evolution
7. **Epilogue: Hello Dumper** - CSV data export

Each act includes:
- 🤔 **Pre-thinking prompts** to activate prior knowledge
- ⚖️ **Design decision points** where you make choices
- 💡 **Understanding checks** to assess comprehension
- 🎯 **Reflection sections** to consolidate learning

## 🗄️ Database: SQLite

This tutorial uses **SQLite** as the database backend. SQLite is Django's default and offers several advantages for learning:

- **Zero configuration** - works out of the box
- **File-based** - your database is just a `db.sqlite3` file
- **Perfect for development** - no separate server needed
- **Built into Python** - no additional installation required

For production deployments with multiple concurrent users, you'd typically use PostgreSQL or MySQL, but SQLite is ideal for this tutorial's scale (270 records).

## 💡 Learning Philosophy

This tutorial follows these principles:

### Socratic Method
Rather than telling you what to do, your AI assistant asks questions that lead you to discover solutions yourself.

### Encouraging Growth Mindset
Mistakes are learning opportunities. Your assistant will help you debug by asking questions, not just giving answers.

### Active vs. Passive Learning
You'll make real decisions, predict outcomes, and explain concepts—not just follow instructions.

### Understanding Over Completion
The goal isn't to finish quickly, but to deeply understand each concept.

## 🎓 What You'll Learn

### Technical Skills
- Django project structure and configuration
- SQLite database management
- Django ORM (Object-Relational Mapping)
- Database migrations and schema evolution
- Custom management commands
- Admin interface customization
- User authentication and permissions
- CSV data import/export

### Developer Thinking
- Data modeling and schema design
- Trade-off analysis in technical decisions
- Debugging through hypothesis testing
- Reading and interpreting error messages
- Version control with Git
- Code organization and best practices

## 🔧 Troubleshooting

### AI Assistant Not Following Claude.md Guidelines

If your assistant isn't asking questions or being Socratic:

1. Make sure `Claude.md` is in the root directory
2. Explicitly ask: "Please guide me through this tutorial using the approach in Claude.md"
3. Remind them: "I want to learn through discovery, not just instructions"

### Python/Django Errors

Your AI assistant will help you debug! Instead of giving up:

1. Read the error message carefully
2. Discuss with your assistant: "What does this error mean?"
3. Form hypotheses about what might be wrong
4. Test your theories

### Environment Issues

If you're having trouble with Python/pipenv:

- **Codespaces users**: Environment should work automatically
- **Local users**: Verify Python 3.9+ with `python --version`
- Check pipenv installation: `pipenv --version`

## 📚 After Completing the Tutorial

### Extend Your Project

Try these challenges:

- Add a field to track whether invitations were accepted/declined
- Implement data validation (e.g., birth dates can't be in the future)
- Add bulk import/export functionality
- Create custom admin actions (e.g., "Assign to reporter")
- Add filtering by decade of birth

### Continue Learning

- [Official Django Tutorial](https://docs.djangoproject.com/en/4.0/intro/tutorial01/)
- [Django Girls Tutorial](https://tutorial.djangogirls.org/)
- [Two Scoops of Django](https://www.feldroy.com/books/two-scoops-of-django-3-x) (book)
- [Test-Driven Development with Python](https://www.obeythetestinggoat.com/) (book)

### Share Your Work

- Tweet about what you built: #DjangoLearning
- Write a blog post about your experience
- Help others in Django community forums
- Contribute to open-source Django projects

## 🙏 Credits

**Original Tutorial by:**
- [Ben Welsh](http://palewi.re/who-is-ben-welsh/)
- Ken Schwencke
- [Dana Amihere](http://damihere.com)

**Interactive Version:**
- Adapted for Claude Code interactive learning
- Enhanced with Socratic teaching methodology
- Updated for Django 4.0+ and SQLite

**Inspired by:**
- LA Times Oscar diversity investigation
- [Sandra Poindexter](http://www.latimes.com/la-bio-sandra-poindexter-staff.html) and [Doug Smith](http://www.latimes.com/la-bio-doug-smith-staff.html)
- [Matt Wynn's](http://mattwynn.net/) NICAR presentation

## 📄 License

This tutorial is open source and available for educational use. The Academy invitee data is from public reporting by the LA Times.

## 🤝 Contributing

Found a bug or have an improvement? Contributions welcome!

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 🌟 Why This Tutorial?

Learning to code is hard. Learning alone is harder. This tutorial combines:

- **Real-world data journalism** project
- **AI-assisted learning** that adapts to you
- **Socratic teaching** that builds deep understanding
- **Hands-on practice** with immediate application

You're not just learning Django—you're learning how to think like a developer.

Ready to begin? Open `docs/index.rst` and start your interactive journey! 🚀

---

**Original Tutorial Documentation:** [first-django-admin-umd.readthedocs.org/](http://first-django-admin-umd.readthedocs.org/)

**Questions or Issues?** Ask your AI assistant or file an issue at [github.com/NewsAppsUMD/first-django-admin-umd/issues/](http://github.com/NewsAppsUMD/first-django-admin-umd/issues/)
