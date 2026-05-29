---
title: "Outreach Hub"
publishDate: "1 October 2021"
description: "Outreach specialists at Cityblock were doing their jobs twice: once on the phone with members, and again afterward to document everything. They were juggling 4+ tabs, a handful of Google Sheets, and a care platform that was not built for them. We fixed that."
tags: ["Cityblock Health", "Design Lead", "User Research", "SaaS", "Onboarding"]

---

# Background
Cityblock is a value-based healthcare company that’s focused on the Medicaid and dually eligible population. They serve those with the most complex needs, and often with the least resources, in the way they deserve to be treated: with respect, compassion, dignity, and time.  

## Problems
- **Cityblock members do not know that they have Cityblock’s coverage** and need to be contacted and onboarded (“outreach” and “consented”). 
    - Our members may be distrustful of us; we're often starting at zero with them. 
- **Cityblock was rapidly scaling, and scaling across markets.** The outreach team struggled with a manual and complex onboarding process. 
    - Each market did things a little differently. All the differences needed to be taken into account and operationalized. 
    - They needed to decrease the time it took to onboard a member *and* reduce the time it took to train an outreach specialist (OS), no matter their location.
    - OS leads needed more visibility into the work
- **Outreach had a workflow, but it was not integrated into Commons (Cityblock’s care system).** They used too many tools to keep track of it and had to duplicate work to hand-off a member. 
    - The care team manages their members in Commons. The outreach team used it, but it wasn't built for their purposes.
### Users  
1. Outreach Specialists (OSs)  
2. Outreach Leads  
### Stakeholders
The Head of Member Engagement and Operations leadership  
### Member Activation & Trust Team  
My Role: Lead designer (IC)  
My Squad: 1 engineer lead (Dan) 1 PM (Ari and then Bobbi)  
Support: Mike (research advisor and MA&T lead), Neves (design team lead)  

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
>I think her overwhelming positive attitude made me just actually join before I could get off the phone with her because she was just too nice. And you wouldn't want to be mean to her.

-- *Recently consented member*

## OS Leads and Stakeholder Interviews
- **Biggest need: Integrated tools for tracking OS performance and smart campaign experimentation**
    - They use a ton of Google sheets for tracking OS performance, but that data stays in Sheets.
    - We need a tool that will pull in our data, claims/other medical data, and our internal research model to surface appropriate engagement tactics.
    - We can also get smarter about OS superpowers. Some leads *know* they have OSs who are especially effective with specific member groups (like pregnant people, older adults, etc.). Integrating that data into the member-assignment model could significantly improve efficiency and conversion rates.
    - OS performance is more complex than our tools can track right now.
- **They want to be able to cut down on training time and remove the amount of decisions an OS has to make.**
    - Clear workflows within Commons, so OSs always know what the next step is
    - Reduce the OS mental load by providing scripts and tests (like flu shot campaigns)
    - Relevant member information (what they might be struggling with the most)
    - OSs need to be able to connect with a member. They don't necessarily need to be health professionals.

![Workflow diagram](./outreach-hub/existingworkflow.jpg)  

## Software research

### Commons
- Technically, Commons had most of what the OSs needed, but everything lived on different pages. And because of poor performance (it loaded lots of other data too), it could not be used on the phone.
- OSs relied on their memory, not the data in front of them, to have a discussion with members.

### Point of Sale Software
The insight that unlocked the MVP concept: POS software does something we weren't doing. It keeps everything relevant on one page and makes data collection easy and standardized. We could shorten the time it takes to consent a member by documenting during the call, so OSs could talk with the member while also gathering accurate information.
![Coffee POS on Dribbble](./outreach-hub/POS1.png)  
[Source](https://dribbble.com/shots/15629660-Kopinan-POS-System-for-Coffee-Shop)  
![Toast Central](./outreach-hub/POS2.png)  
[Source](https://posquote.com/best-restaurant-management-system-online-pos-posquote)  

# MVP
The member’s outreach page is the base of the outreach and intake workflows in Commons. It contains shortcuts and widgets to facilitate easier outreach phone calls and member handoffs. 
![Outreach Hub](./outreach-hub/outreach.png)

## Feature Prioritization
1. **Validate and streamline workflows with Stakeholders** - what work is actually necessary, what can be simplified across markets.  
Stakeholders didn't know all the complexity across markets and workflows. We aligned on the outreach needs. They were close to the existing flow, but we agreed to do less manual tracking wherever possible.
2. **Where are the biggest inefficiencies?** Like double documentation and all of the different tabs and clicking within Commons.
3. **How can we get better data while reducing user effort?** New KPIs: # of tabs open and # of Sheets/market. 
4. **Work with eng partner (Dan) to find the easy wins** - He wrote a script to duplicate the notes so Commons still worked, but the user could do half the work. We did this before actually building a proper fix so we can immediately reduce the work and build a little trust with the OSs. 
5. **Rank features by asking the OS’s,** “What is the worst part of your job?” Attitude impacts the outreach success, so the better moods we can get the OSs in, the more effective they'll be (also, it's the nice thing to do) 

## MVP Features
Two research findings shaped everything: outreach specialists were doing their work from memory, and they were documenting every call twice. The features below are organized around those two problems. Some widgets — phone numbers, consent documents, assessments — reduce friction, but Notes and Outreach History are what changed how the job actually felt.
### Notes
![Notes animation](./outreach-hub/outreachnote.gif) 
- This is where OSs document the member call. 
- This note replaces launching the Outreach / Intake modal from Actions. 
- If an OS consents a member, then they can also add a handoff template 
### Outreach & Claims History
![History animation](./outreach-hub/claimshistory.gif) 
- **Outreach History** gives a snapshot of who on the Cityblock team the member has spoken to thus far. This helps The OSs to pick up where other conversations left off.
- **Claims History** is shortcut to get a picture of a member’s history and recent care.
- You can click to expand and read details.
### Associated Phone Numbers
![Phone number list](./outreach-hub/phonenumbers.png) 
- The phone number with the star in a circle is the member’s primary phone number.
- The other numbers are from the Member Info page.
- This widget gathers any numbers that might help the OS reach the member
- OSs can now click the phone icon on the right to call (instead of copying the number and pasting it into the calling app).
### Verbal Member Consent Documents
![Conset document list](./outreach-hub/verbalconsents.png) 
- OSs no longer have to scroll through the many documents in a member's profile; this widget is a shortcut to the consent documents completed over the phone. 
- They can click the document to open and complete.
- All other consent documents are still in the “Documents” page on the member’s profile. 
- After MVP, we planned to cheat some performance problems by pre-filling the forms - the OS would say the member consented, then generate all the proper documents with a click. 
### Team
![Teams widget](./outreach-hub/Team.gif) 
- This widget helps the OS know what is still incomplete - they can click the yellow button to add an emergency contact.
- They can add any type of the member’s team from this widget by clicking the plus icon in the top right corner.
### Assessments & Tools
![Tools - new](./outreach-hub/assessment1.png) 
![Tools - in progress](./outreach-hub/assessment2.png) 
- This widget is another shortcut to commonly used Assessments & Tools (preventing the OS from navigating away and needing to search for the desired tool).
- OSs can also view previously completed Assessments & Tools or continue editing a draft.
### Quality Opportunities
![List of opportunities](./outreach-hub/qualityopps.png) 
- Quality opportunities are another way to approach discussing a member’s needs. The OS can try scheduling open quality opportunities to get the member onboard.

## Rollout
Our team had one launch goal: every OS would try it at least once in the first two weeks after release. To make that happen, we made the new page as approachable as possible and kept the product team highly accessible. It is hard to change a daily workflow when performance metrics stay the same.
1. Kickoff meeting with training materials
2. Pendo tutorials and surveys
3. Feedback Slack channel for all OSs — they need to have a voice!

# Impact and Additional Learnings
The KPIs told an interesting story. Call volume and conversion increased, but not for our highest-need members. That gap mattered. Those members required more research time, and our performance metrics were actively working against that. This project prompted real conversations with stakeholders about incentive structures — something I don't think would have surfaced without the data we could now see inside Commons.
On the ground, OSs referred to the new page as "our page." We eliminated the need for roughly 5 Google Sheets per market and 4 tabs per outreach session. New OSs used it exclusively. Leads told us it reduced training time and increased their confidence in new hires, so they could focus more on the human side of the work, which was the point.

## KPIs
- **Increase conversion rate (specifically our highest need members)** 
    - We did increase conversion rate, but not for our highest need members
    - Our highest need members simply need more research and we need to incentivise that appropriately. 
- **Increase call volume** 
    - We significantly increased efficiency and OSs were able to increase their calls per day. 
    - We learned that call volume as the main OS performance indicator did not mean we consented more high-need members.
- **Reduce time spent on research** 
    - Research on “easy” consents was reduced, but highest need members was not impacted by this.
    - Our highest need members require additional research, and we need to have the OSs that excel in research focus on these members.
- **Adoption**
    - All the markets used the new page, new OSs used it exclusively and most old OSs used it too (I also reached out to any stragglers to understand more)
 
---
> Many thanks to the MA&T team, Kim D. and all the OSs and Leads who let me into their work. 