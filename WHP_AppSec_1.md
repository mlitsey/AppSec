# We Hack Purple - Applicaiton Security 1

## Application Security Goals

- Inventory 
    1. Take a complete inventory of all software. APIs, WebApps, Serverless, etc.. 
    2. Keeping track of all web assets is extremely valuable. 
- Finding Vulnerabilities
    1. In running code, written code, 3rd party code (libraries, plug-in's). 
    2. Ability to quickly fix issues. 
- Knowledge to fix what has been found
    1. Developer Education, supporting documentation, etc. 
    2. Modernize and learn to eliminate bugs (ex. cross site scripting)
- Effective Tooling
    1. Which tools do we need, and how do we select them? Proof of concept on 3+ tools. 
    2. Automate as much as possible. Part of ci/cd pipleline, scan monthly, etc. 
- Education and Reference Materials
    1. Technical library, Online training, Formal training, Lunch and Learn
    2. Advocacy Program, Security champions program 
- Give Developoers Security Tools
    1. Scan apps
    2. Fix criticals and highs
    3. Send to security for more indepth testing
    4. Put power into software developers hands (self service)
    5. Possibly write own tools, libraries, frameworks
- Security Activities during SDLC (software development life cycle)
    1. Add to each stage of SDLC
    2. Requirements, Design, Coding, Testing, Deployment, Maintenance
    3. Little activites make a big difference
    4. Security sprint
    5. Partnership model (security engineer is assigned to help team)
- Incident Response
    1. IR team understands AppSec or knows when to call the AppSec team
    2. Implement tooling to prevent or detect 
    3. Job specific training for each team in IT 
    4. Why they sould turn over to AppSec (prevent accidental harm)
- Continuous Improvement
    1. Ways of DevOps
        - Emphasize efficiency of entire system
        - Have really fast feedback
        - Continuous Improvement
    2. Metrics, Experimentation, Feedback
    3. Looking for patterns and trends
    4. Discuss with Dev team on how to improve (quarterly?)
- Example 1
    1. Measure current security posture and address any fires
    2. Scan all web apps with DAST tool
    3. Assess top 3 vulnerabilities
    4. Provide a lesson on to 3 (next 3 months do Lunch&Learn, videos, wiki, workshop, OWASP)
    5. Work with teams to eliminate vulnerabilities (be persuasive and communicate clearly)
    6. Then eliminate the high vulnerabilities over the next 6 months.
- Example 2
    1. Get everyone on the same field.
    2. Create repeatable, automated processes that don't interrupt the software development process
    3. All code in the same repository
    4. AppSec team can run tests on the code with automation (GitLab, GitHub, Bit Bucket, ) 6 months using lots of persuasion and management buy in 
    5. Weekly software composition analysis and secret scanning (3-6 months expected). This will show out of date frameworks and libraries, breaking licenses on, and show security vulnerabilities.  
    6. Secret scanning will show if we have any in code. (Hash, password, connection string, API key, )
    7. Weekly SAST (static application security scanning) scans. Check whole repo and have someone check results where there is time (make time)
    8. Automate scans to open tickets on critical and high issues. Beware of false positives. 6 months on criticals, eventually move to highs. 
    9. Penetration test on top 3 mission critical systems, then fix the fires. 
- Example 3
    1. Raise security awareness through the organization and promote positive culture change. 
    2. Possibly create a Security Champion Program. Train them on code review and threat modelling (can be done in about 6 months). Spend another 6 months threat modelling their apps. 
    3. Review each pull request for security. 
    4. Secure Code training for everyone. Will raise awareness, change the culture, and assist the security champions. 
    5. Provide Documentation Support for anything devs are doing. Create a secure coding guideline, web app security requirements, secure design teaching sessions, create a best practices document.
- Setting your goals
    1. https://media2-production.mightynetworks.com/asset/38482339/Your_AppSec_Program_Training_Course_Assignment_1_setting_goals.pdf

## AppSec Activities - Basics

- Different AppSec activities
    1. Strategy : overall campaign plan (goals)
    2. Tactics : actual means used to gain an objective (AppSec activities)
- VA Scans and Secrutiy Assessments
    1. Vulnerability Assessment Scans
        - "Run a scan" - automated tool for quick assessment (low effort and will miss things)
        - DAST (dynamic application security testing), web proxy, web app scanner are examples
    2. Vulnerability/Security Assessments
        - talking to people, assessing whole system, running multiple tools, verifying all security components
- Threat Modelling
    1. What are the threats to the system
        - Mitigate, Reduce, Accept, and document
        - How would they do it?
        - What does this app do?
        - What could go wrong?
        - What keeps you up at night?
        - What could go wrong?
        - How would you hack your app?
    2. Methodologies
        - S.T.R.I.D.E.
        - P.A.S.T.A.
        - Attack Trees
        - others exist that can be used
    3. Talk with stakeholders!
        - What risks exist?
        - How to stop them?
        - Document!
- Secure Code Review and SAST
    1. Manual process
        - Jr. checks in code and Sr. checks for security issues before check off (peer review)
    2. SAST (static application security testing)
        - automated tools
    3. Attempting to find vulnerabilities in your custom code
- Software Composition Analysis (SCA)
    1. Software Composition Analysis (SCA) is the verification of your 3rd party components. Think frameworks, plugins, Nuget packages, libraries. All of that code you didn't write is still code that could cause you harm.
    2. Perform manually or with a tool yearly to ensure security is updated
- Penetration Testing
    1. Hackers check software to see what can be exploited

## AppSec Activities - Intermediate

- Developer Education and Advocacy Programs
    1. 