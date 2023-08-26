class DeveloperProfile {
    private name: string;
    private experience: string;
    private specialization: string[];
    private projectsCompleted: number;
    private clientsServed: string[];
    private contact: {
        phone: string;
        email: string;
    };
    private socialLinks: {
        linkedin: string;
        facebook: string;
        twitter: string;
        instagram: string;
        github: string;
    };
    
    constructor(name: string, experience: string, specialization: string[], projectsCompleted: number, clientsServed: string[]) {
        this.name = name;
        this.experience = experience;
        this.specialization = specialization;
        this.projectsCompleted = projectsCompleted;
        this.clientsServed = clientsServed;
        this.contact = {
            phone: "+9231820980309",
            email: "absarali701@gmail.com"
        };
        this.socialLinks = {
            linkedin: "https://www.linkedin.com/in/hafiz-absar-ali/",
            facebook: "https://www.facebook.com/absardotdev",
            twitter: "https://twitter.com/home",
            instagram: "https://www.instagram.com/absardotdev/",
            github: "https://github.com/absar-ali"
        };
    }
    
    getSkills(): string[] {
        const skills: string[] = [
            // Website Development
            "HTML", "CSS", "JavaScript", "jQuery", "AJAX", "TypeScript", "React.js", "Next.js",
            "Tailwind CSS", "Chakra UI", "ShadCn UI", "WordPress", "Shopify", "Wix",
            "PHP", "Node.js", "Express.js", "tRPC", "Prisma", "Drizzle", "NextAuth", "Clerk",
            "RESTful APIs", "T3 Stack (Web)", "MERN (Web)",
            
            // Flutter Mobile App Development
            "Flutter", "Dart Programming", "Provider", "Bloc", "GetX",
            "Firebase", "SQLite (local database)", "RESTful APIs", "GraphQL",
            "Flutter Animations Libraries", "Push Notifications", "In-App Purchases",
            "MVVM (Flutter)", "Responsive Design",
            
            // Databases & ORM
            "Supabase Postgres", "Vercel Postgres", "Planet-Scale DB",
            "Firestore", "MongoDB", "Microsoft SQL Server", "SQL Lite"
        ];
        return skills;
    }
    
    getAchievements(): string[] {
        const achievements: string[] = [
            "Top-rated Upwork developer for cutting-edge web solutions",
            "Innovation-driven problem solver",
            "Committed to quality, on-time delivery, and client satisfaction",
            "Embrace growth, feedback, and new ideas",
            "Proficient in app development, architectural patterns, Git",
            "Fiverr Level Two Seller, continuously expanding skill set"
        ];
        return achievements;
    }
    
    getProfileSummary(): string {
        return `Hi there, I'm ${this.name}, an experienced developer with ${this.experience} of experience in crafting exceptional web and mobile solutions. My specialization includes ${this.specialization.join(', ')}.
        Throughout my career, I've successfully completed ${this.projectsCompleted} projects for clients around the world, serving entrepreneurs, startups, and established companies.
        My commitment to quality, innovative problem-solving, and proficiency in various technologies has earned me a reputation for delivering top-notch results.`;
    }
    
    getContactDetails(): string {
        return `Feeling uncertain about your upcoming web projects? Let's have a chat and find the perfect solutions together for your next web adventure.
        📱 ${this.contact.phone}
        ✉️ ${this.contact.email}`;
    }
    
    getSocialLinks(): string {
        return `Connect with me on:
        - [LinkedIn](${this.socialLinks.linkedin})
        - [Facebook](${this.socialLinks.facebook})
        - [Twitter](${this.socialLinks.twitter})
        - [Instagram](${this.socialLinks.instagram})
        - Check out my [GitHub](${this.socialLinks.github})`;
    }
}

const absarAli = new DeveloperProfile(
    "Absar Ali",
    "3+ years",
    ["Flutter", "Android", "PHP", "NodeJS"],
    60,
    ["Entrepreneurs", "Startups", "Founders", "CEOs"]
);

const skills = absarAli.getSkills();
const achievements = absarAli.getAchievements();
const profileSummary = absarAli.getProfileSummary();
const contactDetails = absarAli.getContactDetails();
const socialLinks = absarAli.getSocialLinks();

console.log(profileSummary);
console.log("Skills:", skills);
console.log("Achievements:", achievements);
console.log(contactDetails);
console.log(socialLinks);
