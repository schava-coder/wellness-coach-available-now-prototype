# Wellness Coach · Available Now prototype

Interactive member-web concept, published for review. All availability, credits, appointments, chat and calls are simulated. No production account or backend is connected.

## Open in your browser

- Prototype: https://schava-coder.github.io/wellness-coach-available-now-prototype/
- Guided walkthrough: https://schava-coder.github.io/wellness-coach-available-now-prototype/?guide=1

No account, installation or download is required. The HTML includes its own font, public coach imagery, styles and application code. The five coaches are a representative sample roster across specialties.

## 1. See where the feature fits

1. Select **Discover** in the coaching tabs.
2. Find the new Available Now callout beneath the featured coach.
3. Select **Explore available coaches**, or use the **Available Now** tab directly.
4. Browse the sample coaches together. Specialty selection is optional. You can search by name, filter by language/specialty, or switch **Available now only** on and off.
5. Open a coach's photo or name to inspect their profile. Busy and offline coaches remain available for scheduled booking.

## 2. Request a specific coach

1. Choose **Connect now** on Amy's card, or open her profile and choose **Connect now**.
2. Select **30 minutes / 1 credit** or **60 minutes / 2 credits**. These are example prototype prices.
3. Optionally enter a goal, such as preparing for a difficult conversation.
4. Check the readiness/consent box and select **Request Amy**.
5. Watch the waiting state. With the default scenario and auto-play enabled, acceptance is simulated after approximately seven seconds, followed by about three seconds of preparation.
6. Your balance stays unchanged while matching. It decreases only when the simulated booking is ready.
7. Select **Check audio & join**. Try the microphone and camera controls, then select **Join session**.
8. The call screen is a still-image simulation. No camera, microphone, recording or actual call is activated.
9. Select **End session**, confirm, optionally rate the session and select **Done**.
10. Inspect the completed session in **My Coaching**, or book a follow-up.

## 3. Ask the app to find someone

1. Return to **Available Now** and select **Find me a coach**.
2. Choose the duration and language, optionally add a goal, check the readiness/consent box, then submit.
3. No category selection is required. The request is offered to an eligible available coach.
4. Follow the same acceptance, preparation and join steps.
5. For a pooled match, another eligible coach may be tried after a decline. For a specific-coach request, the member is asked before moving to another coach.

## 4. Cancel, recover a request or book for later

- While waiting, select **Cancel request** and confirm. Demo credits remain available.
- Select **Keep my request** to return to waiting, or **Keep browsing while we connect** to close the dialog without cancelling.
- Reopen your active request from the green status banner. Refreshing the same browser tab restores the request when browser session storage is available.
- Choose **Book a session** on a busy/offline coach, or open **Book** and choose a coach.
- Select duration, date and time, then **Confirm session**. The simulated appointment appears in **My Coaching**. No calendar invitation is sent.
- A one-off session does not replace the assigned program coach.

## 5. Review fallback scenarios

Open **Prototype controls** at the lower right, then **Scenarios**. Choose a case, close the controls and start a new request. Changing the case clears the active request and resets the demo balance.

| Scenario | How to try it | Expected result |
| --- | --- | --- |
| Successful connection | Choose a coach or Find me a coach. | Acceptance, preparation and a ready session. |
| Coach declines · find another | Use Find me a coach. | Another eligible coach is tried. With a specific-coach request, alternatives are offered for the member to choose. |
| Coach does not respond | Request a specific coach or use Find me a coach. | A direct request expires after about nine seconds. A pooled request tries up to three offers over roughly twenty-seven seconds, then offers scheduled booking. |
| No coaches available | Inspect the directory and toggle Available now only. | Coaches stay discoverable for later booking; the availability-only view has a clear empty state. |
| Insufficient credits | Start a request and submit the form. | No request is sent; a benefits/credit message is shown. |
| Session setup fails | Submit a request and let the simulated coach accept. | Preparation fails; credits stay available and scheduled booking is offered. |
| Coach becomes unavailable | Start a pooled or specific-coach request. | A pooled match retries; a direct request asks the member to choose an alternative. |

## 6. Control the coach response manually

1. Open **Prototype controls → Scenarios**.
2. Choose **Successful connection** and turn **Auto-play coach responses** off.
3. Close the controls and submit a member request.
4. Open **Prototype controls → Coach response**.
5. Choose **Accept request**, **Decline**, or **Simulate request timeout**.
6. After accepting, choose **Session ready** or **Setup fails**.
7. Close the reviewer controls and continue the member flow.
8. On narrow screens, close the request dialog with X to reach reviewer controls. The active-request banner reopens the dialog.

## 7. Start over or read the design rules

- **Prototype controls → Scenarios → Reset prototype** restores the sample directory and eight demo credits.
- **Prototype controls → Scenarios → Read the reviewer walkthrough** opens the detailed guide inside the app.
- **Prototype controls → Design notes** explains the proposed matching, credit and continuity rules.
- A new browser tab starts a separate demo session. No shared database is used.

## Scope

The prototype demonstrates the member-web journey. Other product modules are outside its scope. Public coach names/photos and illustrative copy provide visual grounding; Alex Morgan and all member activity are fictional. No production account details, private source captures, credentials, health records or real session notes are published.
