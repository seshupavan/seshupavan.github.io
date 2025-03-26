---
title: "How to make better speech therapy applications?"
date: 2025-03-26
slug: "speech-therapy-apps"
description: "Insights from a start-up, hundreds of conversations and self-reflection."
keywords: ["gohugo", "hugo", "go", "blog"]
draft: false
tags: ["speech therapy apps", "stuttering", "stammering", "product"]
summary: Insights from a start-up, hundreds of conversations and self-reflection.
---

I recently wrapped up my work as a product engineer at a startup focused on creating a speech therapy app for stuttering and other speech disorders. As a Person Who Stutters (PWS) myself, I was fortunate to be part of a team exploring technology that could help people like us. Although the startup didn’t succeed, I still believe in the core ideas behind making a better speech therapy app for adults who stutter. These ideas come from hundreds of conversations with PWS worldwide, discussions with Speech-Language Pathologists (SLPs), surveys, and my own research.
<br> I want to document these ideas in this blog post before moving on to the next stage of my career or for someone working in this field might find them useful. Some ideas may be well known but hard to implement due to corporate constraints, while others might offer fresh insights into what users actually want. Finally, because AI is evolving so rapidly in speech therapy, I’ve left a few open-ended questions for you to explore.

## Fundamentals of Speech Therapy Apps
Whether you’re building a speech therapy app using advanced AI or a simpler rule-based system, the fundamentals remain the same. Here are a few key ideas:
 
### Educate Your Users
 Many people begin a speech therapy program hoping their stutter will completely disappear. That’s an understandable goal—stuttering can affect relationships, social life, and job opportunities. With the right therapy, exercises, and guidance, it’s possible to reduce stuttering frequency or gain more fluency, but it’s unlikely to vanish entirely. So, how do we communicate this clearly?
<br> Invest in honest, transparent education. Right from the start, here are some suggestions:
- Clearly explain what speech therapy can realistically achieve, and what it cannot promise or deliver.
- Clarify that stuttering might never fully go away for most people, but its severity and impact can often be reduced significantly over time.
- Educate users on the psychological role of anxiety, the common nature of relapse, and help set grounded expectations about therapy outcomes.
- Avoid misleading marketing promises like “Become fluent in X months,” which can create false hope and eventual disappointment.
- Emphasize that fluency achieved during therapy sessions doesn't always transfer directly to real-life conversations, especially in high-pressure environments.

### Speech AI Isn’t Perfect Yet
Building machine learning systems to match or replace human SLPs is still a long road. Consider the data limitations: the gold standard dataset, [Apple’s SEP-28k](https://machinelearning.apple.com/research/stuttering-event-detection), includes just 40 hours of speech, mostly from American males. We fine-tuned the  Whisper base model on SEP-28k to detect five major disfluencies, and it performed well in validation. However, its performance dropped significantly when tested with diverse accents, tones, and real-life situations. This is just one example of how limited our current pure AI methods are for stuttering diagnosis.
<br> No two disfluencies are exactly alike, making generalization tough. Researchers are even exploring [multimodal approaches](https://arxiv.org/abs/2406.06964)—combining video and audio to detect stuttering—but such methods are still in early research and not ready for broad adoption.

### One Size Won’t Fit All
Stuttering manifests differently in every individual, shaped by personal history, environment, and triggers etc. Categorizing stuttering into breathing patterns, anxiety levels, or avoidance behaviours might help structure a program, but it won’t solve each user’s unique challenges. A more effective strategy is to understand each person’s background such as how stuttering developed, in which scenarios it worsens, and other personal factors through complex questionnaires or maybe an human SLP taking it.
<br> Customization through technology is key for effective therapy results whether AI-based or a personalized plan and Ignoring individual needs can lead to ineffective therapy.

## Fluency:  A Necessary but ticklish goal.
Current speech therapy literature emphasizes acceptance, avoidance reduction, changing self-beliefs, and societal awareness around stuttering. However, many PWS still value fluency because it often translates to better career prospects, more confidence, and improved relationships—though the level of fluency desired varies from person to person. Our experience-sampling surveys also found that self-rated fluency correlates strongly with emotional well-being.
<br> Despite debates about prioritizing fluency, it remains a practical area where technology can help so It’s important to reconsider how we approach fluency using technology. 

### Rethink Course Design
Apps like Stamurai started the trend of offering multiple techniques in one session: breathing exercises, reviewing past techniques, learning new ones, etc. Several apps now do something similar. The downside is that users may be overwhelmed, with little time to practice existing techniques before moving on to new ones.
<br> A better approach starts from the course design itself, here are few ideas:
- Break fluency training into smaller, focused, and clearly defined modules (e.g., gentle onset, prolongation, pull-outs, and light contacts).
- Let users fully master one technique at a time before gradually introducing the next for smoother learning.
- Provide detailed, scenario-based real-life application guides to help users transfer techniques into everyday speaking contexts.
- Users will also benefit from a user-friendly interface providing real-time feedback, progress charts, and gentle reminders. These design elements reinforce daily practice habits, celebrate small wins, and encourage consistency through positive reinforcement.
- Educate users about Relapse in stuttering, why it happens, normalize it and include specific recovery strategies and coping tools.

### Don’t Overload with Techniques
Overloading people with 10 or more speech therapy techniques can be counterproductive. They may struggle to decide which technique to use in a given situation. Additionally, apps often can’t tailor which techniques are best suited for each person, so they end up listing everything. This approach can overwhelm users, creating a cognitive burden that discourages consistent practice and long-term engagement.
<br> As the well-known SLP, C. Woodruff Starkweather put it, people who stutter (PWS) must often choose between two discomforts when picking fluency shaping techniques: the discomfort of stuttering VS the discomfort of adopting an unfamiliar way of speaking. Many PWS eventually give up because speaking differently from everyone else feels unnatural and exhausting. Instead of piling on techniques, it’s more effective to focus on a small, core set that you and your SLP team truly believe in. Start with those, iterate based on real user feedback, and help people bridge the difficult gap between practicing in isolation and applying those tools in everyday life. Often, PWS already know plenty of techniques they just struggle to carry them into realworld conversations.
### Go Beyond Fluency
Many companies design speech therapy apps with the assumption that fluency alone will solve everything. But by adulthood, stuttering has usually already affected many areas of a person's life—such as their relationships, self-image, emotional well-being, and even their core sense of identity. So building an app that focuses only on fluency means ignoring the broader challenges people who stutter actually face.
<br> A more helpful approach is to include additional content that addresses these deeper layers. For example, you could create courses on communication skills (like how to navigate group conversations or presentations), emotional regulation (how to handle shame, anxiety, or anger), or the basics of cognitive behavioral therapy (CBT), which helps users reframe unhelpful thought patterns.
<br> These should be tailored depending on the demographic you're targeting—whether it's young adults starting their careers or older individuals who have experienced a lifetime of speech difficulties. Ultimately, a truly effective speech therapy app should prepare users for life, not just help them become fluent within the confines of their bedroom

## The Bigger Picture

Speech therapy is also about addressing the complex human experience of stuttering. As users grow older, their relationship with stuttering becomes more nuanced where It’s no longer just about fixing speech but learning how to live fully with it. Below are two ideas that can make your app truly meaningful and long-lasting.

### Community and Acceptance
The concept of acceptance for stuttering, to put it simply, means acknowledging your current situation and learning to work from there with a sense of equanimity. This idea has become central in many therapy approaches, particularly those rooted in Acceptance and Commitment Therapy (ACT) and acceptance-based Cognitive Behavioural Therapy (CBT). These models emphasize starting where you are and then focusing on living a meaningful life despite it. While these approaches are increasingly included in speech therapy apps through educational content, video lessons, or blog posts, many users still struggle to emotionally connect with these concepts. They often engage with the material in isolation, without a space to reflect or relate it to real experiences.
<br> That’s why any speech therapy app should consider building spaces for genuine connection. Acceptance, in practice, is not something you learn alone—it’s something you grow into when you're surrounded by people who share your experiences. Apps can create this through community features like Discord servers, weekly group calls, or built-in discussion forums. These environments help users relate to others, express themselves, and feel less alone. When people begin to see themselves in others’ stories, acceptance becomes more than a concept—it becomes a felt experience. From that sense of shared understanding, real motivation and long-term progress are more likely to take root.
<br> Finally, you can consider referring your users to non-profits that are actively working to empower people who stutter around the world through community therapy such as [The Indian Stammering Association](https://stammer.in/home/), [National Stuttering Association](https://www.westutter.org/), [STAMMA](https://stamma.org/) etc etc....

### Invest in Assistive Technology
Do you know why many apps still fail to attract or retain users despite the best UX, AI, and therapy design? Because speech therapy, while helpful, often goes against human instinct. Most people who stutter didn’t choose it but something happened to them. While some benefit from therapy, for others, especially those with severe stuttering, trying harder only makes life more frustrating. Sometimes, no matter how well-designed the product is, it’s just not what the person needs at that point in life. 
<br> I once spoke to a 30-year-old man who had stuttered his whole life. When I asked him, what features are you expecting from us and he replied, "I want an AI that can make my restaurant reservations or help me during interviews." For him, stuttering wasn’t something he needed to fix anymore—he’d accepted it. But he still faced occasional barriers like in a job interviews or booking a table at a restaurant. That conversation shifted my perspective. Sometimes, what people need isn’t more therapy—they need assistive tech that helps them live life without constantly worrying about their speech. Let it be a browser extension for interviews or a tool that rephrases/soothes speech, this might be the next frontier in supporting people who stutter.