[![Typing SVG](https://readme-typing-svg.demolab.com?font=FIre+Code&weight=800&size=24&duration=2000&pause=100&multiline=true&repeat=false&random=false&width=435&height=60&lines=Hey+there!+I'm;DANG+HUU+LOC+%F0%9F%91%8B)](https://git.io/typing-svg)

<a href="https://www.facebook.com/loc.yen.512/" target="_blank" rel="noopener noreferrer">![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white)</a>
<a href="mailto:dhuuloc8818@gmail.com" target="_blank" rel="noopener noreferrer">![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)</a>
<a href="https://www.linkedin.com/in/the-witcher-knight" target="_blank" rel="noopener noreferrer">![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)</a>
<a href="https://stackoverflow.com/users/14512647/loc-dang" target="_blank" rel="noopener noreferrer">![Stack Overflow](https://img.shields.io/badge/-Stackoverflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white)
</a>

```typescript
interface Developer<T extends TechStack> {
  code<R>(project: Project<T>): Result<R>;
  learnNewTech<N extends Technology>(tech: N): Developer<T & N>;
}

type TechStack = Record<string, Technology[]>;
type Technology = string;
type Project<T extends TechStack> = {
  name: string;
  requiredTech: T;
};
type Result<R> = Promise<R>;

class Person<T extends TechStack> implements Developer<T> {
  private readonly name: string;
  private readonly age: number;
  private readonly interests: string[];
  private skills: T;

  constructor() {
    this.name = "Dang Huu Loc";
    this.age = 25;
    this.interests = [
      "Programming",
      "Mechanical Keyboard",
      "Workspace setting up",
      "New technologies",
    ];
    
    // Type-safe skill definition
    this.skills = {
      'Programming Language': ['Go', 'Java', 'JS/TS', 'Dart'],
      'Framework': ['NestJS', 'Gin Gonic', 'Flutter'],
      'Database': ['Postgres', 'MySQL', 'MongoDB', 'Redis', 'Timescale'],
      'Platform': ['Docker', 'Kubernetes', 'AWS'],
      'Tools': ['Git', 'Intellij IDEA', 'VS Code', 'ChatGPT', 'Claude'],
    } as T;
  }

  public code<R>(project: Project<T>): Result<R> {
    console.log(`${this.name} is coding ${project.name}!`);
    return new Promise<R>((resolve) => {
      // Simulate coding process
      setTimeout(() => {
        resolve({} as R);
      }, 1000);
    });
  }

  public learnNewTech<N extends Technology>(tech: N): Developer<T & N> {
    console.log(`${this.name} learned ${tech}!`);
    return this as unknown as Developer<T & N>;
  }

  public getSkills(): T {
    return this.skills;
  }
}

const me = new Person();
me.code({ 
    name: "Awesome Go Microservice", 
    requiredTech: { 'Programming Language': ['Go', 'Typescript'] } 
});
```

----
