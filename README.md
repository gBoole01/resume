# My Resume

This repository contains my resume in JSON format.

JSON Resume is a community driven [Open Source Initiative](https://jsonresume.org/schema) to create JSON-based standard for resumes.

You can visit their [GitHub repository](https://github.com/jsonresume) for more information.
Don't forget to leave a star if you like the project. ⭐️

## JSON Resume Interface

```typescript
interface Resume {
    basics: Basics;
    work: Work[];
    volunteer: Volunteer[];
    education: Education[];
    awards: Award[];
    certificates: Certificate[];
    publications: Publication[];
    skills: Skill[];
    languages: Language[];
    interests: Interest[];
    references: Reference[];
    projects: Project[];
}

interface Basics {
    name: string;
    label: string;
    image: string;
    email: string;
    phone: string;
    url: string;
    summary: string;
    location: Location;
    profiles: Profile[];
}

interface Location {
    address: string;
    postalCode: string;
    city: string;
    countryCode: string;
    region: string;
}

interface Profile {
    network: string;
    username: string;
    url: string;
}

interface Work {
    name: string;
    position: string;
    url: string;
    startDate: string;
    endDate: string;
    summary: string;
    highlights: string[];
}

interface Volunteer {
    organization: string;
    position: string;
    url: string;
    startDate: string;
    endDate: string;
    summary: string;
    highlights: string[];
}

interface Education {
    institution: string;
    url: string;
    area: string;
    studyType: string;
    startDate: string;
    endDate: string;
    score: string;
    courses: string[];
}

interface Award {
    title: string;
    date: string;
    awarder: string;
    summary: string;
}

interface Certificate {
    name: string;
    date: string;
    issuer: string;
    url: string;
}

interface Publication {
    name: string;
    publisher: string;
    releaseDate: string;
    url: string;
    summary: string;
}

interface Skill {
    name: string;
    level: string;
    keywords: string[];
}

interface Language {
    language: string;
    fluency: string;
}

interface Interest {
    name: string;
    keywords: string[];
}

interface Reference {
    name: string;
    reference: string;
}

interface Project {
    name: string;
    startDate: string;
    endDate: string;
    description: string;
    highlights: string[];
    url: string;
}
```
