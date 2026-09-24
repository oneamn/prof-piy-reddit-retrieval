# prof-piy-reddit-retrieval
Public documentation for the read-only Reddit integration used by my private personal AI research assistant.

## Overview

Prof. Piy is a private personal research assistant that runs on my own infrastructure.

This integration uses Reddit as one of several public information sources when a research query benefits from community discussions, firsthand experiences, product feedback, recurring complaints, practical workarounds, or user opinions.

Reddit access is strictly **read-only**.

The application is a personal, non-commercial project and is not offered as a public Reddit service.

## What the Application Does

When I submit a research question to my personal assistant, the application may:

- Search relevant public Reddit posts.
- Retrieve public post content.
- Retrieve public comments and discussion threads.
- Review multiple public discussions relevant to a research question.
- Identify recurring themes, experiences, complaints, opinions, or practical observations.
- Preserve links or references to the original Reddit content where appropriate.
- Summarize relevant Reddit discussions as part of a broader personal research response.

Reddit is only one source within the assistant's research workflow.

The application may also use public websites, official documentation, academic sources, YouTube, and other appropriate sources depending on the research question.

## Reddit API Usage

The application is designed to use authenticated Reddit API access through OAuth.

The production integration uses a Python service and may use the PRAW library to communicate with Reddit's API.

The application will:

- Use OAuth authentication.
- Use a descriptive User-Agent.
- Respect applicable API rate limits.
- Access only the public Reddit content required for a research query.
- Keep Reddit access read-only.

## Read-Only Access

The application does **not** automate actions on Reddit.

It does not:

- Create Reddit posts.
- Submit comments.
- Vote or manipulate votes.
- Send private messages or chat messages.
- Follow users.
- Join communities.
- Moderate subreddits.
- Create Reddit accounts.
- Modify or delete Reddit content.
- Run advertising campaigns.
- Perform automated engagement with Reddit users.

The application only retrieves relevant public information.

## AI and Machine Learning Use

Reddit content retrieved through this integration is **not used to train, fine-tune, or build an AI or machine-learning model**.

The application may use an AI model to analyze and summarize information retrieved for the user's immediate personal research query.

Retrieved Reddit content is used as source material for answering that query, rather than as model-training data.

## Data Usage

The application is intended for low-volume personal research.

Reddit data is not:

- Sold.
- Licensed to third parties.
- Used to build commercial datasets.
- Redistributed as a Reddit dataset.
- Used for advertising profiles.
- Used for automated user profiling.
- Used for AI model training.

The application attempts to retain only the information necessary for the research workflow and source provenance.

Where appropriate, the original Reddit URL or source reference is preserved so the information can be traced back to its public source.

## Deployment

The production application is privately self-hosted on infrastructure controlled by the application owner.

The architecture is approximately:

```text
Personal User
     |
     v
Personal AI Assistant
     |
     v
Research Agent
     |
     v
Read-Only Source Retrieval Service
     |
     v
Reddit OAuth API
```

The source-retrieval component is not a publicly accessible Reddit service.

## Why This Application Runs Outside Devvit

This application is an external personal research assistant rather than an application designed to run inside the Reddit user experience.

It does not provide:

- an interactive Reddit app,
- a Reddit game,
- a moderation application,
- subreddit-specific UI,
- or an experience embedded within Reddit.

Its purpose is limited to authenticated, read-only retrieval of relevant public Reddit discussions from an external private Python service.

For this reason, the application requires external Data API access rather than functioning as a Devvit application.

## Security

Production API credentials are never included in this public repository.

The application keeps credentials and tokens outside source code using private server-side configuration.

This repository intentionally contains:

- no Reddit client secret,
- no OAuth refresh token,
- no passwords,
- no server credentials,
- no private infrastructure configuration.

## Non-Commercial Project

This is a personal and non-commercial project.

The Reddit integration is used only by the owner of the personal assistant for personal research and information retrieval.

It is not currently offered as:

- a paid product,
- a Reddit data service,
- a commercial analytics platform,
- or a public API.

## Source Code

The production source code and infrastructure configuration are private.

This repository exists to publicly document:

- the purpose of the application,
- how Reddit data is used,
- the read-only nature of the integration,
- privacy and security practices,
- and the application's intended API usage.

No production credentials or private infrastructure are published here.

## Contact

For questions regarding this application or its Reddit API usage, please contact the repository owner through GitHub.
