```dart
// Hello there, Welcome! 👋

```dart
class Profile {
  constructor() {
    this.name = 'Your Name';
    this.experience = '3+ Years in Crafting Digital Experiences';
    this.focus = ['Flutter', 'Web Dev', 'Mobile Apps'];
    this.email = 'your.email@example.com';
    this.phone = '+123 456 7890';
    this.location = 'Global Citizen 🌍';
  }

  get skills() {
    return {
      languages: ['Dart', 'JavaScript', 'PHP', 'Node.js'],
      frameworks: ['Flutter', 'React.js', 'Express.js', 'Next.js'],
      databases: ['Firebase', 'MongoDB', 'SQL'],
      tools: ['Git', 'VS Code', 'Figma'],
      interests: ['UI/UX Design', 'App Security', 'Innovation']
    };
  }

  get socialLinks() {
    return {
      linkedin: 'https://www.linkedin.com/in/your-linkedin',
      twitter: 'https://twitter.com/your-twitter',
      instagram: 'https://www.instagram.com/your-instagram',
      website: 'https://www.yourwebsite.com'
    };
  }

  get hireMe() {
    return 'Open to exciting collaborations. Let\'s build the future together!';
  }
}

const developer = new Profile();
