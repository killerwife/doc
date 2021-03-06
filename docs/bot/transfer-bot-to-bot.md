---
id: transfer-bot-to-bot
sidebar_label: Transfer between bots
title: How to transfer a bot to other bot
---

Let's imagine that you want to have several bots and one for each subject.

For example:

 - BotA - Is your first bot where you give welcome and common questions.
 - BotB - is for tech support
 - BotC - is for Customer Care
 - BotD - is for Billing 

You can not transfer directly from **one bot to another bot**,  just like you transfer to an operator.
But one bot can include the context that you made in another.
 
### How to do it

You have to edit the BotB using _These bot logic applies also_: selecting the parent Bot logic what you want to include.

**In this example** BotB include all the logic that you make in BotA so:
- When one visitor uses  BotA only BotA logic is available
- When one visitor uses BotB, is available all logic that you made in BotB and also BotA (so browsing BotB you can *EXECUTE TRIGGER *  using a BotA trigger).

![Including other bot](/img/bot/including-other-bot.png)

:::tip
Remember that when you edit one Bot logic (no matter where it was made), you are editing the same logic for every bot it is included, **they are just included-linked not copied**
:::

:::warning
If in BotB you edit BotA and choose a trigger from BotB and later go to edit directly BotA you won't see chosen trigger in BotA. You should construct bot in a such way that you would not need to choose triggers directly in BotA.
:::
