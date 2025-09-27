---
layout: project
type: project
image: img/SoftEng/SoftEngRobotPage.png
title: "CS Software Engineering Project"
# date: Mar 2023 – May 2023
start: 2023-03-01
end:   2023-05-31
published: true
labels:
  - Java
  - Software Engineering
  - Frontend
  - UML
  - Documentation
summary: "Worked in a 10-person team to build an application for Brigham & Women’s Hospital, integrating robotics with manual and vision-based control."
---
<figure class="text-center">
  <img class="img-fluid d-block mx-auto" src="{{ site.baseurl }}/img/SoftEng/signInPage.png" alt="Hospital service request platform with integrated robotics.">
  <figcaption>
    Main sign in page for the built website.
  </figcaption>
</figure>

## Project Overview
As part of **CS3733-D23: Software Engineering**, our team *Overworked Ouroboroi* (Max Berman, Alexander Presser, Allen Cheung, Anuragi Thapliya, Keelan Boyle, Mike McInerney, Nicholas Leslie, Ruba Khan, Sophia Woodward, Stephen Fanning) created a **hospital service request system** for Brigham and Women’s Hospital. The application supports map editing, meal and supply delivery, therapy requests, signage management, and **robot-assisted navigation**. It connects to a PostgreSQL database and includes staff/admin login functionality.

I contributed in two main areas:  
- **Robotics Integration** – Programmed a robot to track AprilTags and navigate toward service request locations, allowing the system to dispatch and guide a physical delivery robot:contentReference.  
- **Documentation Analyst** – Led the creation of the **User Manual** and final project documentation, ensuring that system design, usage instructions, and technical details were clearly explained.  

---

## Key Features
- **Service Requests:** Supports requests for meals, office supplies, flowers, therapy animals, and IT services. 
- Implemented error-handling popups for service requests and login failures to improve robustness.   
- **Map Editing & Pathfinding:** Editable hospital maps with pathfinding via A*, BFS, DFS, and Dijkstra algorithms. Visual and text directions grouped by floor improved usability.  
- **Robotics Control:**  
  - Integrated FRC-based robot hardware with RoboRIO, Limelight vision, and AprilTag detection.  
  - Added a **robot control panel** for autonomous navigation and service request fulfillment.  
- **Backend & Cloud:**  
  - PostgreSQL database with DAO and Facade patterns.  
  - Real-time announcements via **AWS Lambda** + **WebSockets**.  
  - OAuth login via AWS Cognito.  
- **Documentation & Testing:** Produced detailed documentation and user instructions, including UML diagrams, ERDs, and user-facing help resources.  

---

## Documentation
Due to confidentiality agreements, only the final User Manual can be shared.

- 📄 [User Manual](https://drive.google.com/file/d/1nF99FmbLhDC38xVBiWGtXGipFiVNjTtq/view?usp=sharing)  