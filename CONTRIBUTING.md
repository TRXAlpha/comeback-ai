# 🤝 Contributing to Comeback AI

> **Thank you for your interest in contributing to Comeback AI!** ✨  
> *Made with ❤️ by Pink Pixel - "Dream it, Pixel it"*

We're excited to have you join our community of contributors who are helping to make negativity a thing of the past through AI-powered humor! 

---

## 🎯 **Table of Contents**

- [Code of Conduct](#-code-of-conduct)
- [Getting Started](#-getting-started)
- [Development Setup](#️-development-setup)
- [Contributing Guidelines](#-contributing-guidelines)
- [Pull Request Process](#-pull-request-process)
- [Issue Guidelines](#-issue-guidelines)
- [Coding Standards](#-coding-standards)
- [Testing](#-testing)
- [Documentation](#-documentation)
- [Community](#-community)

---

## 🌟 **Code of Conduct**

By participating in this project, you agree to abide by our community standards:

### ✅ **Do's**
- 💝 Be respectful and inclusive
- 🎭 Keep the humor positive and entertaining
- 🤝 Help others learn and grow
- 🐛 Report bugs constructively
- 💡 Share ideas thoughtfully
- 🎉 Celebrate others' contributions

### ❌ **Don'ts**
- 🚫 Use inappropriate or offensive language
- 😠 Engage in personal attacks or harassment
- 🗂️ Share private information without permission
- 💔 Discourage new contributors
- 🚨 Submit harmful or malicious content

---

## 🚀 **Getting Started**

### **First Time Contributing?**
Welcome! We're thrilled to have you. Here's how to get started:

1. 🍴 **Fork the repository**
2. 📥 **Clone your fork locally**
3. 🌿 **Create a feature branch**
4. ✨ **Make your changes**
5. 🧪 **Test thoroughly**
6. 📝 **Submit a pull request**

### **Areas We Need Help With**
- 🎭 **New Personas** - Creative character ideas and personalities
- 🎨 **UI/UX Improvements** - Design enhancements and user experience
- 🔧 **Bug Fixes** - Resolving issues and improving stability
- 📖 **Documentation** - Better guides, examples, and explanations
- 🌍 **Internationalization** - Multi-language support
- ⚡ **Performance** - Optimization and speed improvements
- 🧪 **Testing** - Test coverage and quality assurance

---

## 🛠️ **Development Setup**

### **Prerequisites**
- **Node.js** 18+ ([Download](https://nodejs.org/))
- **npm** or **yarn**
- **Git** ([Download](https://git-scm.com/))
- **VS Code** (recommended) with TypeScript extension

### **Setup Steps**

```bash
# 1. Fork and clone the repository
git clone https://github.com/YOUR_USERNAME/comeback-ai.git
cd comeback-ai

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev

# 4. Open in browser
# Visit http://localhost:5173
```

### **Available Scripts**

| Command | Description |
|---------|-------------|
| `npm run dev` | 🚀 Start development server |
| `npm run build` | 🏗️ Build for production |
| `npm run lint` | 🔍 Run ESLint |
| `npm run lint:fix` | 🔧 Fix ESLint issues |
| `npm run preview` | 👀 Preview production build |

---

## 📋 **Contributing Guidelines**

### **Types of Contributions**

#### 🐛 **Bug Fixes**
- Small fixes that resolve existing issues
- No new features or breaking changes
- Include tests when possible

#### ✨ **Features**
- New functionality or enhancements
- Discuss in an issue before implementing
- Include documentation and tests

#### 📚 **Documentation**
- README improvements
- Code comments and JSDoc
- Examples and tutorials

#### 🎨 **Design**
- UI/UX improvements
- Visual enhancements
- Responsive design fixes

### **Contribution Size Guidelines**

| Type | Description | Review Time |
|------|-------------|-------------|
| 🐾 **Small** | 1-10 lines changed | 1-2 days |
| 🐕 **Medium** | 10-100 lines changed | 3-5 days |
| 🦁 **Large** | 100+ lines changed | 1-2 weeks |

---

## 🔄 **Pull Request Process**

### **Before Submitting**
1. ✅ Ensure your code follows our coding standards
2. 🧪 Run tests and fix any failures
3. 🔍 Run linting and fix any issues
4. 📖 Update documentation if needed
5. 🎯 Keep changes focused and atomic

### **PR Title Format**
Use conventional commit format:
```
type(scope): description

Examples:
feat(personas): add Robot Butler persona
fix(audio): resolve playback issues on Safari
docs(readme): update installation instructions
style(ui): improve mobile responsiveness
```

### **PR Description Template**

```markdown
## 🎯 Description
Brief description of what this PR does.

## 🔧 Type of Change
- [ ] 🐛 Bug fix
- [ ] ✨ New feature
- [ ] 💥 Breaking change
- [ ] 📚 Documentation update
- [ ] 🎨 Style/UI improvement

## 🧪 Testing
- [ ] Tests pass locally
- [ ] Manual testing completed
- [ ] New tests added (if applicable)

## 📋 Checklist
- [ ] Code follows style guidelines
- [ ] Self-review completed
- [ ] Documentation updated
- [ ] No merge conflicts

## 📷 Screenshots (if UI changes)
[Add screenshots here]
```

---

## 🐛 **Issue Guidelines**

### **Bug Reports**
Use our bug report template:

```markdown
**🐛 Bug Description**
Clear description of what went wrong.

**🔄 Steps to Reproduce**
1. Go to '...'
2. Click on '...'
3. See error

**✅ Expected Behavior**
What should have happened.

**🖥️ Environment**
- Browser: Chrome 120
- OS: Windows 11
- Device: Desktop

**📷 Screenshots**
[Add screenshots if helpful]
```

### **Feature Requests**
Use our feature request template:

```markdown
**✨ Feature Description**
Clear description of the proposed feature.

**🎯 Problem to Solve**
What problem does this solve?

**💡 Proposed Solution**
How would you implement this?

**🔄 Alternatives Considered**
Other solutions you've thought about.

**📊 Additional Context**
Any other relevant information.
```

---

## 💻 **Coding Standards**

### **TypeScript**
- ✅ Use TypeScript for all new code
- 📝 Define interfaces for complex objects
- 🎯 Prefer type safety over `any`
- 📋 Use meaningful variable names

### **React**
- 🧩 Use functional components with hooks
- 🎨 Follow React best practices
- 🔄 Use React Router for navigation
- 🎭 Leverage Framer Motion for animations

### **Styling**
- 🎨 Use Tailwind CSS utility classes
- 📱 Mobile-first responsive design
- 🌈 Follow existing color scheme
- ⚡ Optimize for performance

### **Code Structure**
```typescript
// ✅ Good - Clear, typed, documented
interface PersonaProps {
  name: string;
  voice: string;
  onSelect: (persona: string) => void;
}

export function PersonaCard({ name, voice, onSelect }: PersonaProps) {
  const handleClick = () => {
    onSelect(name);
  };

  return (
    <div className="persona-card" onClick={handleClick}>
      <h3>{name}</h3>
      <p>Voice: {voice}</p>
    </div>
  );
}
```

### **File Organization**
```
src/
├── components/     # Reusable UI components
├── pages/         # Route-based page components
├── lib/           # Utility functions and helpers
├── types/         # TypeScript type definitions
└── hooks/         # Custom React hooks
```

---

## 🧪 **Testing**

### **Testing Strategy**
While we don't have comprehensive tests yet, we encourage:

- 🔧 **Manual Testing**: Test your changes thoroughly
- 📱 **Cross-browser**: Check Chrome, Firefox, Safari
- 📲 **Responsive**: Test on mobile and desktop
- ♿ **Accessibility**: Ensure keyboard navigation works

### **Future Testing Plans**
- 🎯 **Unit Tests**: Jest + React Testing Library
- 🔄 **Integration Tests**: API integration testing
- 🎭 **E2E Tests**: Playwright for user workflows
- ⚡ **Performance**: Lighthouse CI for performance monitoring

---

## 📖 **Documentation**

### **Code Documentation**
- 📝 Use JSDoc for complex functions
- 💬 Add inline comments for tricky logic
- 📋 Document component props with TypeScript

### **User Documentation**
- 📖 Update README for new features
- 🎯 Include usage examples
- 📷 Add screenshots for UI changes
- 🔗 Link to relevant resources

---

## 🌍 **Community**

### **Getting Help**
- 💬 **Discord**: @sizzlebop
- 🐙 **GitHub Discussions**: Coming soon
- 📧 **Issues**: For bugs and feature requests
- 🌐 **Website**: [pinkpixel.dev](https://pinkpixel.dev)

### **Recognition**
We appreciate all contributions! Contributors will be:
- 🏆 Listed in our contributors section
- 🎉 Mentioned in release notes
- ✨ Featured on our website (with permission)
- 💝 Sent virtual high-fives and gratitude

---

## 🎨 **Persona Contribution Guidelines**

### **Creating New Personas**
When adding new personas to `personas.json`:

```json
{
  "name": "Quirky Character Name",
  "voice": "voice_id",
  "prompt": "Detailed personality description that guides AI behavior..."
}
```

#### **Persona Requirements**
- 🎭 **Unique Personality**: Distinct from existing personas
- 🎤 **Voice Assignment**: Use available voice IDs
- 📝 **Clear Prompt**: Detailed instructions for AI behavior
- 😊 **Positive Humor**: Keep it entertaining, not harmful
- 🎯 **Target Audience**: Consider broad appeal

#### **Voice Options**
Available voices: `alloy`, `echo`, `fable`, `onyx`, `nova`, `shimmer`, `coral`, `verse`, `ballad`, `ash`, `sage`, `amuch`, `dan`

---

## 🚀 **Release Process**

### **Version Numbering**
We follow [Semantic Versioning](https://semver.org/):
- 🔧 **PATCH** (0.1.X): Bug fixes
- ✨ **MINOR** (0.X.0): New features
- 💥 **MAJOR** (X.0.0): Breaking changes

### **Release Schedule**
- 🗓️ **Regular Releases**: Monthly minor releases
- 🐛 **Hotfixes**: As needed for critical bugs
- 🎉 **Major Releases**: Quarterly feature releases

---

## 🙏 **Thank You**

Every contribution, no matter how small, makes Comeback AI better for everyone. Whether you're fixing a typo, suggesting a new persona, or implementing a major feature, you're helping create something that brings joy and laughter to people worldwide.

**Together, we're turning negativity into comedy, one comeback at a time!** 🎭✨

---

*© 2025 Pink Pixel. All rights reserved.*  
*"Dream it, Pixel it" ✨*

---

**Questions?** Reach out to us:
- 🐙 **GitHub**: [github.com/pinkpixel-dev](https://github.com/pinkpixel-dev)
- 💬 **Discord**: @sizzlebop
- 🌐 **Website**: [pinkpixel.dev](https://pinkpixel.dev) 