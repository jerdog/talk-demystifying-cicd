@snap[midpoint]
# Demystifying CI/CD 
@snapend
---
# Some clever story


---
# Define terms


---
## "DevOps"

![What is devops](assets/img/devops_is_coming.jpeg)

---
## "CI"


---
## "CD"


---
# So about CI/CD...

Note:
I've been part of development teams where code would take weeks or months before it was pushed to testing, and often months before it would be deployed to production. And that was just one team, working on one feature, while other teams worked on other features doing the same thing. It was also not uncommon to be working on a project for a year - only to have it dumped because the business and/or customer had already moved past the need. Who here would prefer slow code delivery cycles? Every technology delivery team wants to increase their code delivery velocity and the quality of the code they push to market.

---
## DevOps Lifecycle

@snap[midpoint]
![width=600](assets/img/devops_lifecycle.png)
@snapend

Note:

 Who here is familiar with the DevOps Lifecycle?



### Add Some Slide Candy

![IMAGE](assets/img/presentation.png)

---?color=linear-gradient(180deg, white 75%, black 25%)
@title[Customize Slide Layout]

@snap[west span-55]
## Customize the Layout
@snapend

@snap[north-east span-45]
![IMAGE](assets/img/presentation.png)
@snapend

@snap[south span-100]
Snap Layouts let you create custom slide designs directly within your markdown.
@snapend

---
@title[Add A Little Imagination]

@snap[north-west span-50 text-center]
#### Engage your Audience
@snapend

@snap[west span-55]
@ul[list-spaced-bullets text-09]
- You will be amazed
- What you can achieve
- With a **little imagination**
- And GitPitch Markdown
@ulend
@snapend

@snap[east span-45]
![IMAGE](assets/img/conference.png)
@snapend

@snap[south span-100 bg-black fragment]
@img[shadow](assets/img/conference.png)
@snapend

---

@snap[north-east span-100 text-pink text-06]
Let your code do the talking!
@snapend

```sql zoom-18
CREATE TABLE "topic" (
    "id" serial NOT NULL PRIMARY KEY,
    "forum_id" integer NOT NULL,
    "subject" varchar(255) NOT NULL
);
ALTER TABLE "topic"
ADD CONSTRAINT forum_id
FOREIGN KEY ("forum_id")
REFERENCES "forum" ("id");
```

@snap[south span-100 text-gray text-08]
@[1-5](You can step-and-ZOOM into fenced-code blocks, source files, and Github GIST.)
@[6,7, zoom-13](Using GitPitch live code presenting with optional annotations.)
@[8-9, zoom-12](This means no more switching between your slide deck and IDE on stage.)
@snapend


---?image=assets/img/code.jpg&opacity=60&position=left&size=45% 100%

@snap[east span-50 text-center]
## Now It's **Your** Turn
@snapend

@snap[south-east span-50 text-center text-06]
[Download GitPitch Desktop @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend

