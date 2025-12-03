# Contributing to ENTR Minor Repository

Thank you for contributing to the ENTR Minor program materials! This guide will help faculty and teaching staff collaborate effectively.

## 🎯 Who Can Contribute

- **Faculty Members**: Course instructors and program leads
- **Teaching Assistants**: TAs assisting with course delivery
- **Program Administrators**: Staff managing curriculum and logistics
- **Guest Instructors**: Industry experts and visiting lecturers

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/aloysiusraj001/ENTR.git
cd ENTR
```

### 2. Create a Branch

Always create a new branch for your changes. Never commit directly to `main`.

```bash
git checkout -b feature/your-feature-name
```

**Branch Naming Conventions:**
- `feature/` - New content or materials (e.g., `feature/week3-slides`)
- `update/` - Updates to existing content (e.g., `update/syllabus-2025`)
- `fix/` - Corrections and bug fixes (e.g., `fix/assignment2-typo`)
- `docs/` - Documentation updates (e.g., `docs/readme-update`)

### 3. Make Your Changes

Edit, add, or remove files as needed. Ensure your changes are:
- **Well-organized**: Follow the repository structure
- **Properly named**: Use clear, descriptive filenames
- **Documented**: Include README files in new folders

### 4. Commit Your Changes

Write clear, descriptive commit messages:

```bash
git add .
git commit -m "Add Week 3 lecture slides on business models"
```

**Commit Message Guidelines:**
- Start with a verb (Add, Update, Fix, Remove, Refactor)
- Be specific and concise
- Reference issue numbers if applicable

**Examples:**
- ✅ `Add assignment 2 rubric and starter code`
- ✅ `Update syllabus with new office hours`
- ✅ `Fix typo in Week 4 slides`
- ❌ `Updated stuff`
- ❌ `Changes`

### 5. Push Your Branch

```bash
git push origin feature/your-feature-name
```

### 6. Create a Pull Request

1. Go to the repository on GitHub
2. Click "Pull requests" > "New pull request"
3. Select your branch
4. Fill in the PR template:
   - **Title**: Clear summary of changes
   - **Description**: What changed and why
   - **Reviewers**: Tag relevant faculty/staff
5. Submit the pull request

### 7. Review and Merge

- Wait for review from program lead or designated reviewers
- Address any feedback or requested changes
- Once approved, the PR will be merged to `main`

## 📝 File Organization

### Directory Structure

Maintain the established structure:

```
ENTR/
├── syllabus/
│   ├── ENTR101_Syllabus_2025.pdf
│   └── ENTR201_Syllabus_2025.pdf
├── slides/
│   ├── week01_introduction.pptx
│   └── week02_ideation.pptx
├── assignments/
│   ├── assignment01/
│   │   ├── brief.md
│   │   ├── rubric.pdf
│   │   └── starter_code/
└── projects/
    └── final_project/
        ├── guidelines.md
        └── template.docx
```

### File Naming Conventions

- **Use lowercase with underscores**: `business_model_canvas.pdf`
- **Include version/date when relevant**: `syllabus_2025_spring.pdf`
- **Be descriptive**: `week03_customer_discovery_slides.pptx` not `w3.pptx`
- **Avoid spaces**: Use `_` instead of spaces

### Folder-Level README Files

Each major folder should contain a `README.md` explaining:
- Purpose of the folder
- How files are organized
- Any special instructions

## ✅ Content Guidelines

### What to Include

- **Course Materials**: Slides, handouts, readings
- **Assignments**: Briefs, rubrics, starter files
- **Projects**: Guidelines, templates, examples
- **Resources**: Reading lists, tool guides, datasets
- **Documentation**: READMEs, guides, notes

### What NOT to Include

❌ **Private Materials**:
- Solution keys or answer sheets
- Grading rubrics with internal notes
- Student submissions or grades
- Confidential institutional documents

❌ **Large Binary Files**:
- Video recordings (link to external storage instead)
- Large datasets (provide download links)
- High-resolution images (optimize first)

❌ **Sensitive Information**:
- Personal contact details
- Login credentials
- API keys or tokens

**Note**: Use the `/admin/` folder for internal materials not meant for student access. This folder can be kept private or added to `.gitignore` if needed.

## 🔍 Code Review Process

### For Contributors

1. **Self-review first**: Check your changes before submitting PR
2. **Test links and files**: Ensure all references work
3. **Check formatting**: Preview Markdown files
4. **Respond promptly**: Address reviewer feedback quickly

### For Reviewers

1. **Review within 48 hours**: Keep workflow moving
2. **Be constructive**: Suggest improvements, don't just criticize
3. **Check for**:
   - Correct folder placement
   - Proper file naming
   - No sensitive information
   - Working links and references
   - Clear documentation

## 👥 Communication

### Getting Help

- **Technical Issues**: Open an issue on GitHub
- **Content Questions**: Contact program lead
- **Urgent Matters**: Email the ENTR team

### Discussion and Feedback

- Use GitHub Issues for:
  - Proposing new materials
  - Reporting errors or inconsistencies
  - Suggesting improvements
- Use Pull Request comments for:
  - Reviewing specific changes
  - Asking clarification questions
  - Discussing implementation details

## 🛡️ Best Practices

### Version Control

- **Commit frequently**: Small, logical commits are better than large ones
- **Pull before pushing**: Always `git pull` to get latest changes first
- **Resolve conflicts promptly**: Don't let merge conflicts accumulate

### Collaboration

- **Communicate changes**: Let team know about major updates
- **Respect existing structure**: Follow established patterns
- **Document your work**: Add comments and READMEs
- **Ask questions**: Better to ask than to guess

### Quality

- **Proofread**: Check for typos and formatting errors
- **Test materials**: Ensure assignments and examples work
- **Maintain consistency**: Use same style as existing content
- **Update related files**: If you change one file, update references elsewhere

## ❓ Common Scenarios

### Adding a New Week of Content

```bash
git checkout -b feature/week5-content
# Add slides, readings, assignments
git add slides/week05_*.pptx resources/week05_readings.md
git commit -m "Add Week 5 content: Market validation"
git push origin feature/week5-content
# Create PR on GitHub
```

### Updating the Syllabus

```bash
git checkout -b update/syllabus-spring2025
# Edit syllabus file
git add syllabus/ENTR101_Syllabus_Spring2025.pdf
git commit -m "Update syllabus: Adjust assessment weights and add office hours"
git push origin update/syllabus-spring2025
# Create PR with detailed changelog
```

### Fixing an Error

```bash
git checkout -b fix/assignment3-typo
# Fix the error
git add assignments/assignment03/brief.md
git commit -m "Fix typo in assignment 3 due date"
git push origin fix/assignment3-typo
# Create quick PR
```

## 📚 Additional Resources

- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- [Writing Good Commit Messages](https://chris.beams.io/posts/git-commit/)

## ⚖️ License

By contributing, you agree that your contributions will be licensed under the same license as the project (see [LICENSE](LICENSE)).

---

**Questions?** Contact the program lead or open an issue on GitHub.
