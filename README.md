
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Linkedin } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="p-6 max-w-4xl mx-auto">
      <header className="text-center mb-10">
        <h1 className="text-4xl font-bold">Shashidhar Akula</h1>
        <p className="text-lg text-gray-600 mt-2">Sr. Full Stack Java Developer</p>
        <div className="flex justify-center space-x-4 mt-4">
          <a href="mailto:shashidharakula14@gmail.com">
            <Button variant="outline"><Mail className="mr-2 h-4 w-4" /> Email</Button>
          </a>
          <a href="https://www.linkedin.com/in/shashidhar-akula-b8a230253" target="_blank">
            <Button variant="outline"><Linkedin className="mr-2 h-4 w-4" /> LinkedIn</Button>
          </a>
        </div>
      </header>

      <section className="mb-10">
        <h2 className="text-2xl font-semibold mb-4">About Me</h2>
        <p className="text-gray-700">
          Full Stack Developer with 9+ years of experience in building and maintaining enterprise applications. Specialized in Java, Spring Boot, Microservices, React, AWS, and Kubernetes. Strong background in designing scalable backend systems and responsive frontend applications.
        </p>
      </section>

      <section className="mb-10">
        <h2 className="text-2xl font-semibold mb-4">Key Projects</h2>
        <div className="grid gap-6">
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-bold">Safeway Warehouse Management</h3>
              <p className="text-gray-700 mt-2">
                Migrated on-prem applications to AWS, refactored legacy monoliths to microservices using Spring Boot, deployed on Kubernetes. Integrated AWS Cognito and API Gateway for secure authentication.
              </p>
              <p className="text-sm text-gray-500 mt-2">Tech Stack: Java 17, Spring Boot, React, AWS, Kubernetes, Jenkins</p>
            </CardContent>
          </Card>

          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-bold">United Health Group Microservices Platform</h3>
              <p className="text-gray-700 mt-2">
                Developed RESTful microservices for healthcare systems, leveraging Spring Boot and deployed on ECS with CI/CD automation using Jenkins and Terraform.
              </p>
              <p className="text-sm text-gray-500 mt-2">Tech Stack: Java 11, Spring Boot, AWS ECS, Terraform, Jenkins</p>
            </CardContent>
          </Card>
        </div>
      </section>

      <section>
        <h2 className="text-2xl font-semibold mb-4">Experience</h2>
        <ul className="space-y-6">
          <li>
            <h3 className="text-xl font-bold">Sr. Full Stack Developer @ Safeway Inc.</h3>
            <p className="text-gray-700">May 2022 – Present</p>
            <ul className="list-disc list-inside text-gray-700 mt-2">
              <li>Led modernization of legacy applications into cloud-native microservices.</li>
              <li>Used React for dynamic UI and Spring Boot for backend microservices.</li>
              <li>Implemented CI/CD with Jenkins and containerized apps using Docker.</li>
            </ul>
          </li>
          <li>
            <h3 className="text-xl font-bold">Java AWS Developer @ United Health Group</h3>
            <p className="text-gray-700">Aug 2020 – Apr 2022</p>
            <ul className="list-disc list-inside text-gray-700 mt-2">
              <li>Developed REST APIs with Spring Boot and deployed to AWS ECS.</li>
              <li>Implemented secure IAM policies, S3 lifecycle rules, and EC2 auto-scaling.</li>
              <li>Utilized Terraform and Jenkins for infrastructure provisioning and deployments.</li>
            </ul>
          </li>
        </ul>
      </section>
    </div>
  );
}
