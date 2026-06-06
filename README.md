# Prompt Engineering Portfolio

| Detail | Information |
|----------|----------|
| **Name** | Ekta Vijay Tiwari |
| **Date** | 4 June 2026 |
| **LLM Used** | ChatGPT-4 |

---

# Part 1: Prompt Design & Iteration

## Scenario A: Technical Explanation

### Goal

Explain recursion to a 10-year-old.

### Initial Prompt

```text
Explain recursion to a 10-year-old.
````

#### Initial Output

```text
# Understanding Recursion (For a 10-Year-Old)

## What Is Recursion?

Recursion is when something **does the same job again and again**, but each time with a **smaller problem** to solve.

Think of it like standing between two mirrors. You see yourself over and over because the image keeps repeating itself.

In programming, a function can even **call itself**. That's recursion!

## A Simple Example: Russian Nesting Dolls

Imagine you have a big doll.

Inside it is a smaller doll.

Inside that one is an even smaller doll.

You keep opening dolls until you reach the tiniest doll that cannot be opened anymore.

That's recursion:

1. Open the doll.
2. If there's another doll inside, open that one too.
3. Keep going.
4. Stop when you reach the smallest doll.

The smallest doll is called the **base case**.

## Why Do We Need a Base Case?

Without a base case, recursion would never stop!

Imagine saying:

"Count down from 10."

10 → 9 → 8 → 7 → ...

Eventually, you reach 0 and stop.

If you never stop, you'd be counting forever!

## Example: Counting Down

Let's count down from 5.

5
4
3
2
1
0

Here's what the recursive thinking looks like:

- Say 5
- Ask yourself to count down from 4
- Say 4
- Ask yourself to count down from 3
- Say 3
- Keep going...
- Stop when you reach 0

## Visualizing It

Starting with 3:

countDown(3)
 └─ countDown(2)
     └─ countDown(1)
         └─ countDown(0)
             └─ Stop!

Each step creates a smaller version of the same problem.

## Real-Life Example

Imagine climbing down a ladder.

To get from step 5 to the ground:

- Go down one step.
- Then solve the same problem from step 4.
- Then from step 3.
- Then from step 2.
- Then from step 1.
- Finally, you're on the ground.

That's recursion in action!

## The Two Rules of Recursion

Every recursive solution needs:

### 1. A Base Case

The condition that tells it when to stop.

Example:

If number is 0, stop.

### 2. A Recursive Step

The part where the function calls itself with a smaller problem.

Example:

Count down from number - 1.

## A Tiny Code Example

def count_down(n):
    if n == 0:
        print("Done!")
    else:
        print(n)
        count_down(n - 1)

count_down(3)

Output:

3
2
1
Done!

## Easy Way to Remember

Recursion is like saying:

"I'll solve this problem by solving a smaller version of the same problem."

And keep doing that until the problem becomes so small that it's easy to finish.

## Summary

- Recursion means a function calls itself.
- It solves a problem by breaking it into smaller versions of the same problem.
- It always needs a **base case** to stop.
- Without a base case, it would run forever.
- Examples include counting down, nesting dolls, and climbing down a ladder.

Think of recursion as a set of tiny helpers, where each helper asks a smaller helper to do the same job until the smallest helper can finish it alone.
```

---

### Refined Prompt – Iteration 1

```text
Explain recursion to a 10-year-old using simple language and a real-life example. Avoid technical terms and keep the explanation under 150 words.
```

#### Iteration 1 Output

```text
# What Is Recursion?

Imagine you have a stack of 5 books and want to count them.

You pick up the top book and say, "That's 1 book." Then you look at the smaller stack underneath and do the same thing again. Each time, the stack gets smaller.

Eventually, there are no books left. That's when you stop.

Recursion is like solving a problem by doing the same simple step over and over on a smaller version of the problem until there's nothing left to do.

A real-life example is opening a set of nested boxes. You open the biggest box, then the smaller box inside it, then the next one, and so on. When you reach the smallest box, you stop.

So, recursion means **repeating the same idea on a smaller version of something until you reach the end.**
```

---

### Refined Prompt – Iteration 2

```text
You are an expert elementary school teacher who specializes in explaining computer science concepts to children.

I am teaching a group of 10-year-olds who have never done any programming before.

Explain recursion using a fun story. Avoid technical jargon, use simple language, explain why recursion eventually stops, and keep the explanation between 150 and 200 words.
```

### Final Output (Iteration 2)

```text
# The Magic Treasure Boxes

One day, Mia found a magical treasure box in her attic. She opened it and was surprised to find another smaller treasure box inside!

Curious, Mia opened the smaller box. Inside was an even smaller treasure box. She opened that one too, and found another.

Each box contained a smaller box, so Mia kept doing the same thing: open the box and look inside.

After a while, she reached the tiniest box of all. When she opened it, there was no other box inside—just a shiny gold coin!

At that moment, Mia stopped opening boxes because there were no more boxes left to open.

Recursion is a lot like Mia's adventure. You do the same action again and again, but each time with a smaller version of the same thing. Just like the boxes got smaller, the problem gets smaller too.

The reason recursion eventually stops is that you reach a point where there is nothing smaller left to work on. In Mia's story, that point was the smallest box with the gold coin inside.

That's how recursion works: repeat the same idea until you reach the stopping point.
```

---

## Scenario B: Professional Email

### Goal

Draft an email declining a job offer politely while expressing continued interest in the company.

### Initial Prompt

```text
Write an email declining a job offer.
```

#### Initial Output

```text
Subject: Job Offer

Dear Hiring Manager,

Thank you for offering me the position. After careful consideration, I have decided not to accept the offer.

I appreciate the opportunity and wish you success in finding the right candidate.

Sincerely,
[Your Name]
```

### Refined Prompt – Iteration 1

```text
Write a professional email declining a job offer politely. Thank the company for the opportunity and express interest in staying connected for future opportunities.
```


#### Iteration 1 Output

```text
Subject: Thank You for the Opportunity

Dear Hiring Manager,

Thank you very much for offering me the position. I sincerely appreciate the time and effort that you and the team invested throughout the interview process.

After careful consideration, I have decided to decline the offer at this time. This was not an easy decision, as I was impressed by the company and the team.

I would like to stay in touch and hope there may be opportunities to work together in the future.

Thank you again for your consideration, and I wish you and the team continued success.

Best regards,
[Your Name]
```

### Refined Prompt – Iteration 2

```text
You are an experienced HR professional who specializes in business communication.

I have received a job offer from a company that I genuinely admire, but I have decided to accept another opportunity that better aligns with my current career goals. I would like to decline the offer professionally while preserving a positive relationship and expressing sincere interest in future opportunities with the company.

Write a professional email of 200–250 words with a warm, respectful, and appreciative tone.
```

### Final Output - (Iteration 2)

```text
Subject: Thank You for the Opportunity

Dear Hiring Manager,

Thank you very much for offering me the opportunity to join your team. I truly appreciate the time, effort, and consideration that you and the interview panel invested throughout the recruitment process.

After careful thought, I have decided to accept another opportunity that more closely aligns with my current career goals and circumstances. This decision was not easy, as I have been genuinely impressed by your organization’s culture, values, and the professionalism demonstrated throughout the hiring process.

I want to express my sincere gratitude for the confidence you placed in me and for the opportunity to learn more about the company. My decision is not a reflection of any shortcomings in the role or organization. On the contrary, my interactions with the team have only strengthened my admiration for the company and its mission.

I hope to stay connected and would welcome the opportunity to be considered for future roles that may align with my experience and career path. I greatly respect the work your organization is doing and would be delighted to cross paths again in the future.

Thank you once again for your understanding and kindness throughout this process. I wish you and the entire team continued success.

Kind regards,

[Your Name]
```

## Scenario C: Creative Content

### Goal

Generate a creative marketing tagline for a new eco-friendly water bottle brand.

### Initial Prompt

```text
Create a tagline for an eco-friendly water bottle brand.
```

#### Initial Output

```text
# Eco-Friendly Water Bottle Brand Taglines

### Tagline Options

1. **Sip Sustainably.**
2. **Hydrate with Purpose.**
3. **Better Water, Better Planet.**
4. **Refill. Reuse. Respect Nature.**
5. **Drink Green, Live Clean.**
6. **Every Sip Makes a Difference.**
7. **Hydration for a Healthier Earth.**
8. **Small Bottle, Big Impact.**
9. **Choose Reuse. Choose Change.**
10. **Refresh Yourself. Protect the Planet.**
11. **Sustainable by Design.**
12. **Pure Hydration, Conscious Living.**
13. **Crafted for You. Kind to Earth.**
14. **Elevate Your Hydration, Reduce Your Footprint.**
15. **Fill. Sip. Repeat.**
16. **Planet-Friendly Hydration.**
17. **Reuse the Future.**
18. **Carry Water, Not Waste.**
19. **Drink Responsibly.**

### Recommended Tagline

**Hydrate with Purpose.**

This tagline highlights both personal well-being and environmental responsibility, making it ideal for an eco-friendly water bottle brand.
```

### Refined Prompt – Iteration 1

```text
Create 5 creative taglines for an eco-friendly water bottle brand. The taglines should be memorable, modern, and emphasize sustainability and reducing plastic waste.
```

#### Iteration 1 Output

```text
# 5 Creative Taglines for an Eco-Friendly Water Bottle Brand

1. **Refill Today, Renew Tomorrow.**
2. **Hydrate Smart, Waste Less.**
3. **Every Sip Saves a Little More.**
4. **Carry Water, Not Plastic Waste.**
5. **Drink Clean. Live Green.**

### Key Theme
These taglines emphasize sustainability, eco-conscious living, and reducing single-use plastic waste while maintaining a modern and memorable appeal.
```

### Refined Prompt – Iteration 2

```text
Our new water bottle brand is designed for environmentally conscious young professionals who want stylish, reusable products that reduce single-use plastic waste.

Create 10 marketing taglines that are creative, memorable, emotionally engaging, and no more than 8 words long. Focus on sustainability, personal impact, and everyday lifestyle benefits.
```

#### Final Output - Iteration 2

```text
# 10 Marketing Taglines for an Eco-Friendly Water Bottle Brand

1. **Style Your Sip, Save the Planet.**
2. **Refill Today. Inspire Tomorrow.**
3. **Every Refill Creates Positive Change.**
4. **Drink Better, Live Greener.**
5. **Sustainability Looks Good on You.**
6. **One Bottle. Endless Positive Impact.**
7. **Hydrate Smart, Waste Less Daily.**
8. **Carry Change Wherever You Go.**
9. **Small Choice, Lasting Difference.**
10. **Refill with Purpose, Every Day.**
```


---

## 1.2 Iteration Documentation 

### Scenario A: Technical Explanation

| Version | Prompt                                                                                                                                                                                                                                                                                                                                                                             | What Changed                                                                                                                              | Why This Improved the Output                                                                                                                                    |
| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **V1**  | `Explain recursion to a 10-year-old.`                                                                                                                                                                                                                                                                                                                                              | N/A                                                                                                                                       | N/A                                                                                                                                                             |
| **V2**  | `Explain recursion to a 10-year-old using simple language and a real-life example. Avoid technical terms and keep the explanation under 150 words.`                                                                                                                                                                                                                                | Added instructions to use simple language, include a real-life example, avoid technical jargon, and limit the response length.            | The output became easier for a child to understand and more focused on the target audience.                                                                     |
| **V3**  | `You are an expert elementary school teacher who specializes in explaining computer science concepts to children. I am teaching a group of 10-year-olds who have never done any programming before. Explain recursion using a fun story. Avoid technical jargon, use simple language, explain why recursion eventually stops, and keep the explanation between 150 and 200 words.` | Added role assignment, audience context, story-based format, explanation of the stopping condition, and a more specific output structure. | The output became more engaging, age-appropriate, and educational. The role and context helped the model tailor the explanation to the needs of young learners. |

### Scenario B: Professional Email

| Version | Prompt | What Changed | Why This Improved the Output |
|----------|----------|----------|----------|
| V1 | `Write an email declining a job offer.` | N/A | N/A |
| V2 | `Write a professional email declining a job offer politely. Thank the company for the opportunity and express interest in staying connected for future opportunities.` | Added professionalism, gratitude, and future networking requirements. | The output became more polite, appreciative, and aligned with professional communication standards. |
| V3 | `You are an experienced HR professional who specializes in business communication. I have received a job offer from a company that I genuinely admire, but I have decided to accept another opportunity that better aligns with my current career goals. I would like to decline the offer professionally while preserving a positive relationship and expressing sincere interest in future opportunities with the company. Write a professional email of 200–250 words with a warm, respectful, and appreciative tone.` | Added role assignment, detailed context, reason for declining, relationship-preservation goal, tone requirements, and length constraints. | The output became more personalized, professional, and realistic. The role and context helped the model generate a nuanced email that effectively balances gratitude, professionalism, and future interest. |

### Scenario C: Creative Content

| Version | Prompt | What Changed | Why This Improved the Output |
|----------|----------|----------|----------|
| V1 | `Create a tagline for an eco-friendly water bottle brand.` | N/A | N/A |
| V2 | `Create 5 creative taglines for an eco-friendly water bottle brand. The taglines should be memorable, modern, and emphasize sustainability and reducing plastic waste.` | Requested multiple options and specified themes such as sustainability and plastic waste reduction. | Produced more varied and relevant taglines while focusing on the brand's environmental mission. |
| V3 | `Our new water bottle brand is designed for environmentally conscious young professionals who want stylish, reusable products that reduce single-use plastic waste. Create 10 marketing taglines that are creative, memorable, emotionally engaging, and no more than 8 words long. Focus on sustainability, personal impact, and everyday lifestyle benefits.` | Added target audience, brand context, emotional objectives, and output constraints. | Generated more distinctive and marketable taglines tailored to the intended customers and brand positioning. |

---


## 1.3 Role and Context Usage

### Scenario A: Technical Explanation
---
#### Role Assignment

> "You are an expert elementary school teacher who specializes in explaining computer science concepts to children."

#### Context Setting

> "I am teaching a group of 10-year-olds who have never done any programming before."
---

### Scenario B: Professional Email
---
#### Role Assignment

> "You are an experienced HR professional who specializes in business communication."

#### Context Setting

> "I have received a job offer from a company that I genuinely admire, but I have decided to accept another opportunity..."

### Scenario C: Creative Content 
---
#### Role Assignment

> "You are an award-winning marketing copywriter who specializes in sustainable consumer brands."

#### Context Setting

> "Our new eco-friendly water bottle brand is designed for environmentally conscious young professionals..."

## 1.3 Role and Context Usage

Role assignment and context setting significantly improved the quality and relevance of the generated outputs across all three scenarios. In Scenario A, assigning the role of an "expert elementary school teacher" and providing context about teaching 10-year-olds helped the model explain recursion in a way that was engaging, age-appropriate, and easy to understand.

In Scenario B, assigning the role of an "experienced HR professional" and providing context about declining a job offer while maintaining a positive relationship with the company resulted in a more professional, thoughtful, and realistic email. The additional context helped the model balance gratitude, professionalism, and future interest.

In Scenario C, assigning the role of an "award-winning marketing copywriter" and providing information about the target audience and brand values enabled the model to create taglines that were more creative, emotionally appealing, and aligned with the company's sustainability mission. The outputs became more targeted and marketable than those generated from generic prompts.

Overall, role assignment helps the model adopt the expertise and communication style required for a task, while context setting provides background information that guides the model toward more relevant and effective responses.

---
