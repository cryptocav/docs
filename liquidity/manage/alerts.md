---
title: Alerts
description: Stay in range, capture more fees. Get notified the moment your position moves out of range.
icon: bell
---

Stop watching charts. Start getting notified.

Orca Alerts let you know the moment any position moves out of range—so you can take action, stay in range, and keep those fees flowing. Set up takes seconds, and you can receive notifications in-app, via Telegram, or by email.

<Info>
Orca Alerts are powered by [Dialect](https://dialect.to), providing fast and reliable real-time messaging infrastructure on Solana.
</Info>

## Why Alerts Matter

With concentrated liquidity, your position only earns fees while the price stays within your selected range. When price drifts outside that range:

- **Your position stops earning** — No trades happen at your price points
- **You might want to rebalance** — Adjust your range to get back in the action  
- **Time is money** — The sooner you know, the faster you can act

Alerts eliminate the need to constantly monitor charts. You'll get a notification the moment something needs your attention.

---

## Opening the Notifications Panel

You can access alerts from anywhere on Orca using the **envelope icon** in the top-right corner of the navigation bar, next to your wallet.

<Frame>
  <img src="/images/alerts-nav-icon.png" alt="Envelope icon in the Orca navigation bar" />
</Frame>

Click it to open the **Notifications** panel, which has three tabs:

| Tab | What It Does |
|-----|--------------|
| **Inbox** | View all your notifications—filter by Alerts or News |
| **Manage Alerts** | See, toggle, or delete your existing alerts |
| **Create Alert** | Set up a new alert for any position |

<Frame caption="The Inbox tab shows all your alert notifications with timestamps and quick links">
  <img src="/images/alerts-inbox.png" alt="Notifications Inbox showing out of range alerts" />
</Frame>

<br />

<Tip>
You can also create an alert directly from a position. On the **Pools** page, click any position to open **Position Details**, then look for the bell icon and "Create an alert for this position" in the Details tab.
</Tip>

<br />

<Frame caption="Create alerts directly from the Position Details sidebar">
  <img src="/images/alerts-position-details.png" alt="Position Details panel showing alert creation option" />
</Frame>

---

## Creating an Alert

Setting up an alert takes just a few seconds:

<Steps>
  <Step title="Open the Create Alert tab">
    Click the envelope icon in the navigation bar, then select the **Create Alert** tab.
  </Step>
  
  <Step title="Select your position">
    Use the dropdown to choose which position you want to monitor. You'll see the pool pair, fee tier, current range, and balance for each position.
  </Step>
  
  <Step title="Name your alert">
    Give your alert a nickname. By default, it uses the pool name (e.g., "SOL/USDC 0.04%"), but you can customize it to something more descriptive.
  </Step>
  
  <Step title="Choose your alert condition">
    Currently, you can set alerts for when your **position moves out of range**. More conditions are coming soon!
  </Step>
  
  <Step title="Set the trigger frequency">
    Choose how often you want to be notified:
    
    | Trigger | Behavior |
    |---------|----------|
    | **Only once** | You'll receive one notification, then the alert is automatically deleted |
    | **Every time** | Get notified each time the condition is met |
    | **Once a minute** | Receive at most one notification per minute while the condition persists |
  </Step>
  
  <Step title="Create your alert">
    Click **Create Alert**. You'll see a confirmation message: "Successfully Created Alert — Your alert has been created."
  </Step>
</Steps>

<br />

<Frame caption="The Create Alert tab with all configuration options">
  <img src="/images/alerts-create.png" alt="Create Alert interface showing position selection, nickname, condition, and trigger options" />
</Frame>

That's it! Your alert is now active and monitoring your position. You'll see a confirmation toast:

<Frame caption="Success! Your alert is ready to go">
  <img src="/images/alerts-success.png" alt="Successfully Created Alert confirmation message" style={{ maxWidth: '400px' }} />
</Frame>

---

## Managing Your Alerts

Head to the **Manage Alerts** tab to see all your alerts at a glance. You can filter by:

- **All** — Every alert you've created
- **Active** — Alerts currently monitoring your positions
- **Inactive** — Alerts you've paused

<Frame caption="The Manage Alerts tab showing your active and inactive alerts">
  <img src="/images/alerts-manage.png" alt="Manage Alerts tab with alert cards showing toggle and delete options" />
</Frame>

Each alert card shows:
- The alert nickname and creation date
- Pool details (pair, fee tier, range, balance)
- Alert condition and trigger frequency
- Toggle switch to enable/disable
- Delete button

### Pause or Resume an Alert

Use the **toggle switch** on any alert to pause it without deleting. Toggle it back on whenever you're ready to resume notifications.

<Frame caption="Toggle alerts on or off without deleting them">
  <img src="/images/alerts-toggle.png" alt="Alert cards showing active and inactive toggle states" />
</Frame>

### Delete an Alert

Click the **trash icon** on any alert. You'll see a confirmation prompt—click **Delete** to confirm, or **Cancel** to keep it.

<Frame caption="Confirm before deleting an alert">
  <img src="/images/alerts-delete.png" alt="Delete confirmation dialog with Cancel and Delete buttons" />
</Frame>

---

## Notification Settings

Click the **gear icon** in the Notifications panel to configure how you receive alerts. You have three options:

<CardGroup cols={3}>
  <Card title="In-App" icon="browser">
    Alerts appear directly in your Inbox when you're using Orca. This is enabled by default for your connected wallet.
  </Card>
  
  <Card title="Telegram" icon="telegram">
    Click **Connect Telegram** to link your account. After connecting, you'll need to subscribe to notifications in Telegram to start receiving alerts.
  </Card>
  
  <Card title="Email" icon="envelope">
    Enter your email address and click **Send Code** to verify. Once confirmed, you'll receive alerts directly in your inbox.
  </Card>
</CardGroup>

<br />

<Frame caption="Configure your notification preferences in Settings">
  <img src="/images/alerts-settings.png" alt="Notification settings showing In-App, Telegram, and Email options" />
</Frame>

<Note>
You can enable multiple notification methods. For example, receive alerts both in-app and via Telegram for redundancy.
</Note>

---

## Viewing Your Notification History

The **Inbox** tab shows all notifications you've received. Each alert notification includes:

- The pool and position that triggered it
- The alert type (e.g., "Out of Range")
- Timestamp of when it occurred
- A **View Pool** link to jump directly to that pool

Use the filter buttons to view **All**, just **Alerts**, or **News** updates from Orca.

---

## Tips for Effective Alerts

<AccordionGroup>
  <Accordion title="Start with 'Only once' for new positions">
    If you're testing the waters or just want a heads-up, use the "Only once" trigger. You'll get one notification and can always create a new alert after.
  </Accordion>
  
  <Accordion title="Use 'Every time' for positions you actively manage">
    For positions where you want to stay on top of every range exit, use "Every time" so you never miss a move.
  </Accordion>
  
  <Accordion title="Use 'Once a minute' for volatile pairs">
    Highly volatile pairs might bounce in and out of range frequently. "Once a minute" prevents notification overload while keeping you informed.
  </Accordion>
  
  <Accordion title="Set up Telegram for instant mobile alerts">
    In-app notifications are great when you're at your computer, but Telegram ensures you get alerts on your phone wherever you are.
  </Accordion>
</AccordionGroup>

---

## What's Coming Next

The Orca team is actively improving alerts. On the roadmap:

- **New & trending pool alerts** — Get notified about hot opportunities
- **Daily LP digests** — A summary of your portfolio's performance

Stay tuned for updates!

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Portfolio Overview" icon="chart-pie" href="/liquidity/manage/portfolio">
    Learn how to monitor all your positions in one place
  </Card>
  
  <Card title="Harvest Your Yield" icon="seedling" href="/liquidity/manage/harvest">
    Collect the fees you've earned from your positions
  </Card>
</CardGroup>
