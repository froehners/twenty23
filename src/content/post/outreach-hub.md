---
title: "Outreach Hub"
publishDate: "1 October 2021"
description: "Building a new workflow hub for outreach specialists in an existing tool."
tags: ["Cityblock Health", "Design Lead", "SaaS", "Onboarding"]

---

# Background
Cityblock is a value-based healthcare company that’s focused on the Medicaid and dually eligible population. They serve those with the most complex needs, and often with the least resources, in the way they deserve to be treated—with respect, compassion, dignity, and time.

## Problems
- Cityblock members do not know that they have Cityblock’s coverage and need to be contacted and onboarded (“outreach” and “consented”). 
    - Our members may be distrustful of us; we're often starting at zero with them. 
- Cityblock was rapidly scaling, and scaling across markets. The outreach team struggled with a manual and complex onboarding process. 
    - Each market did things a little differently. All the differences needed to be taken ito account and operationalized. 
    - They needed to decrease the time it took to onboard a member *and* reduce the time it took to train an outreach specialist (OS), no matter their location.
    - OS leads needed more visibility into the work
- Outreach had a workflow, but it was not integrated into Commons (Cityblock’s care system). They used too many tools to keep track of and had to duplicate work to hand-off a member. 
    - Commons is a healthcare platform, where the care team manages their members. The outreach team used it, but it wasn't built for their purposes.

## Goals 
**Meaningfully improve the efficiency of our engagement funnel**  
Enable outreach specialists to spend less time researching and more on personalized conversations. Provide a guided workflow so that the team doesn’t have to remember each step, reducing documentation gaps, and increasing documentation quality. 

**Personalize outreach conversations to offer more value upfront**  
Surface details about a member and scripts, tips, and resources that will help the outreach team with the initial engagement conversation. Provide a space to operationalize early wins and other engagement experiments. 

**Support a centralized outreach team**  
Simplify workflows for outreach specialists, allow new employees to get up to speed faster, and minimize nuances across markets. 

**KPIs**  
- Increase conversion rate (specifically our highest need members)
- Increase call volume
- Reduce time spent on research
- Adoption (this one's important - working outside of Commons is less safe, but also means we can’t learn as much from their usage)  

# Discovery
Since we wanted a centralized outreach team and process, I had to understand what tools and workflows they were using across markets. We wanted to launch an MVP quickly so we can start getting wins and learnings to build upon. 

## User Interviews + Shadowing Sessions
- **Biggest need: accurate member information, faster**
    -   It often takes more than one outreach session to consent a member, so the OS needs to be able to carry the previous conversation. Knowing the member's history shows legitimacy. 
- **OSs use a lot of different tools and pages in Commons**
    - All the different tools slow them down and makes them need to rely on memory (this allowed for a lot of differences between OSs and didn't allow for controlled experimentation within markets). 
    - Commons had performance issues - it’s too slow to use in real-time
    - They use the calling tool, a script document, tracking Sheets, research tools and notepads for documentation
    - They also have to submit two notes within Commons: One Outreach note, and one Intake note.
    - There is an intake checklist UI, but it is not accurate and not being used
- **Consent conversations are not linear.** OSs often weave various parts of the intake process into natural conversation. 
- Documentation and handoff is very labor-intensive. OSs try to keep calls as short as possible, so **essentially consent workflow happens twice - verbally with the member and then documenting it in the system.**
- The gratification of helping members means the OSs do a lot of extra work without complaint. Their workflows were more inefficient than we realized.
- **The emotional impact of outreach**
    - The best part of an OS’s day is when they get to help (and consent) a member
    - The worst part of conducting outreach is the monotony (lots of ringing with no answers)
    - Often new OSs are more successful than more experienced ones, but it takes time to learn the system and the script
- **OSs need to have energy and enthusiasm when they talk to members**
>“I think her overwhelming positive attitude made me just actually join before I could get off the phone with her because she was just too nice. And you wouldn't want to be mean to her.” 
*- Recently consented member*



## OS Leads and Stakeholder Interviews

## Software research

### Commons
### Point of Sale Software

# MVP

## Feature Prioritization
1. **Validate and streamline workflows with Stakeholders** - what work is actually necessary, what can be simplified across markets.  
Stakeholders didn't know all the complexity across markets and workflows. We aligned on the outreach needs. They were close to the existing flow, but we agreed to do less manual tracking wherever possible.
2. **Where are the biggest inefficiencies?** Like double documentation and all of the different tabs and clicking within Commons.
3. **How can we get better data while reducing user effort?** New KPIs: # of tabs open and # of Sheets/market. 
4. **Work with eng partner (Dan) to find the easy wins** - He wrote a script to duplicate the notes so Commons still worked, but the user could do half the work. We did this before actually building a proper fix so we can immediately reduce the work and build a little trust with the OSs. 
5. **Rank features by asking the OS’s,** “What is the worst part of your job?” Attitude impacts the outreach success, so the better moods we can get the OSs in, the more effective they'll be (also, it's the nice thing to do) 

## Rollout

# Impact and Additional Learnings

#### References + Thanks:
- Huge shoutout to the Member Activation and Trust Team <3
- Kim D. was also an incredible resource! 