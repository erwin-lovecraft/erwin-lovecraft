# Hey there! I'm DANG HUU LOC :wave:

<a href="https://www.facebook.com/loc.yen.512/" target="_blank" rel="noopener noreferrer">![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white)</a>
<a href="mailto:dhuuloc8818@gmail.com" target="_blank" rel="noopener noreferrer">![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)</a>
<a href="https://www.linkedin.com/in/virsavik-dang" target="_blank" rel="noopener noreferrer">![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)</a>
<a href="https://stackoverflow.com/users/14512647/loc-dang" target="_blank" rel="noopener noreferrer">![Stack Overflow](https://img.shields.io/badge/-Stackoverflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white)
</a>

```dart
class Person implements Developer<FullStack> {
  String name;
  String alias;
  int age;
  List<String> interests;
  Map<String, List<String>> skills;
  
  Person({
    this.name = "Dang Huu Loc",
    this.alias = "Virsavik",
    this.age = 23,
    this.interests = const [
      "Programming",
      "Mechanical Keyboard",
      "Workspace setting up",
      "New technologies",
    ],
    this.skills = const {
      'Programming Language': ['Go', 'Java', 'JS/TS', 'Dart'],
      'Framework': ['Flutter', 'SpringBoot', 'Next.js', 'Angular'],
      'Database': ['Postgres', 'MySQL'],
      'Platform': ['Docker', 'Azure', 'AWS', 'Kubernetes'],
      'Tools': ['Git', 'Intellij IDEA', 'VS Code'],
    },
  });


  @override
  void code() {
    print("$name is coding!");
  }

  @override
  void collaborateWithTeam() {
    print("$name is collaborating with the team!");
  }

  @override
  void performCodeReview() {
    print("$name is participating in a code review!");
  }

  @override
  void writeDocumentation() {
    print("$name is writing documentation!");
  }

  @override
  void keepLearning() {
    print("$name is committed to continuous learning!");
  }

  @override
  void optimizeCode() {
    print("$name is optimizing code for performance!");
  }

  @override
  void implementSecurityMeasures() {
    print("$name is implementing security measures!");
  }
}
```
