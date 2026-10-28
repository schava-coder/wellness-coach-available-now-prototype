# Available Now — member and coach interactive prototype

I created a prototype with mock data covering the member app and coach dashboard, so we can review the complete experience before implementation.

- [Open the prototype](https://schava-coder.github.io/wellness-coach-available-now-prototype/)
- [Open the detailed reviewer guide](https://schava-coder.github.io/wellness-coach-available-now-prototype/?guide=1)
- [Start on the coach dashboard](https://schava-coder.github.io/wellness-coach-available-now-prototype/?view=coach)

No sign-in, installation, or download is required. Use sample text only. All availability, requests, balances, appointments, notes, messages, and video are mock data. Nothing changes a real account.

## How to go back and forth

Use **Member app** and **Coach dashboard** in the top reviewer bar. Switching keeps the current request. When switching to the coach during an active request, the receiving coach is selected automatically. **Demo coach** lets you view any of the five sample coaches. For a pooled retry, **Open receiving coach** opens the coach currently receiving the offer.

You can also open this link in two tabs in the **same browser profile**, keeping one on Member app and one on Coach dashboard. Availability, request status, credits, sessions, and saved notes synchronize between those tabs. Different people, browsers, profiles, and devices have independent demo data; this prototype has no shared backend.

Leave **Prototype controls → Scenarios → Auto-play coach responses** off when reviewing both sides. The default is manual. Auto-play is optional for a quick member-only walkthrough; it simulates coach acceptance and the coach joining.

The reset icon in the top bar restores Amy as the selected coach, three available sample coaches, no sessions, and eight credits. Reset affects both tabs. Refreshing restores the saved browser-local data.

## Main walkthrough

1. **Coach dashboard → Available Now.** Turn off the availability switch. Switch to Member app and verify Amy no longer offers Connect now. She remains discoverable for a scheduled booking.
2. Return to **Coach dashboard → Set availability**. Choose **2 hours**, enable **30 and 60 minutes**, and **Save availability**. Switch to Member app; Amy is available again.
3. In **Member app → Available Now**, choose **Connect now** on Amy’s card. Select **30 minutes / 1 credit**, optionally enter “I want a manageable routine this week,” tick the readiness checkbox, and select **Request Amy**.
4. The member waits and still has eight credits. Choose **Review request as coach**, or use the top bar. The coach sees Alex’s goal, duration, language, and a **90-second response window**.
5. Choose **Accept request**. The coach is reserved; another request cannot use that coach. About three seconds later, the mock booking and room are ready. The balance changes to seven once.
6. Switch to **Member app**, open the active session banner, choose **Check audio & join**, try the simulated media controls, and select **Join session with Amy**. The member waits for the coach; no device permissions are requested.
7. Choose **Switch to coach and join**, then **Join session**. Both views now show the same session in progress. Use the top bar to inspect either side. A minimized room can be reopened from the active session banner or Return to session.
8. **End session** from either side. The other view updates. On Coach dashboard, the coach stays unavailable while wrapping up.
9. Enter an optional private note and an optional shared next step, such as “Try a 10-minute walk after lunch three times this week.” Choose **Save & finish wrap-up**. The coach becomes available again only if the switch is on and sufficient time remains.
10. In **Member app → My Coaching → View summary**, verify the shared next step. Private notes appear only in the coach UI. **Coach dashboard → Sessions** shows the same completed session.

## Other scenarios to test

| Scenario | How to try it | Expected result |
| --- | --- | --- |
| Direct request declined | Request Amy, switch to coach, Decline request | Member chooses another coach or books later; no silent substitution and no credits used. |
| Pooled retry | Member → Find me a coach; decline the first offer | Another eligible coach receives the request. Use Open receiving coach to inspect it. |
| No response | Wait 90 seconds, or Prototype controls → Coach response → Simulate request timeout | Direct request ends; pooled request tries another eligible coach. Credits stay available. |
| Cancel while matching | Member → Cancel request → confirm | Incoming coach offer closes. Late acceptance cannot revive it. |
| Cancel after confirmation | Cancel before both participants join | Both views close the booking and mock credits return once. |
| Stop future requests | Coach turns availability off during an accepted session | Current session remains reserved. After wrap-up, coach stays offline. |
| Duration does not fit | Coach sets 45-minute availability, 30-minute session length | Thirty-minute request fits; sixty-minute option is disabled for that coach. Book for later remains available. |
| Calendar conflict | Prototype controls → Scenarios → Coach becomes unavailable; or Coach response → Add calendar conflict | A mock booking twenty minutes away blocks thirty/sixty-minute requests for that coach. Clear calendar conflict to restore capacity. |
| Availability expires | Coach response → Expire this coach’s availability | Switch clears and Connect now disappears. Accepted sessions continue. |
| No available coaches | Scenarios → No coaches available | All five sample coaches can still be explored/booked; Available now only shows a useful empty state. |
| Insufficient credits | Scenarios → Insufficient credits; submit a request | No offer is sent and no credits are consumed. |
| Session setup fails | Scenarios → Session setup fails; request and accept as coach | Preparation fails, both sides update, and the original balance stays available. |
| Join timeout | Confirm a session but do not have both people join for five minutes | Session closes and mock credits return. |
| Scheduled fallback | Book a session → duration/date/time → Confirm session | Mock booking appears in member My Coaching and the selected coach’s Sessions. No calendar invite is sent. |
| Reload/two tabs | Refresh or use two tabs in the same browser profile | Saved state remains and updates synchronize. Reset clears both tabs. |

A scenario change resets the current request, history, availability, and balance. It retains your auto-play preference. Set Successful connection or use Reset when returning to the main review.

## What feedback to give

- Is it clear how coaches set a window and stop new requests?
- Are goal, language, duration, and the response window enough to decide whether to accept?
- Can the member tell who is being asked, when acceptance happens, when credits are used, and who still needs to join?
- Are decline, retry, cancellation, calendar conflict, and scheduling fallbacks understandable?
- Does the wrap-up make the shared next step easy to find while keeping the private note out of the member UI?
- Does the addition fit the existing dark member app and light coach dashboard?

Pricing (30 minutes/one credit, 60 minutes/two credits), a five-minute buffer, a ninety-second response window, a five-minute join window, and pre-session credit returns are **proposed prototype rules for review**. This is not a statement of current production policy.

The new connected feature is clickable; unrelated coach Programs, Clients, Chats, and SOP Assistant modules are outside this review. Browser-local note separation demonstrates the UI only, not production authorization. Real implementation needs server-side eligibility/entitlements, atomic reservations, coach presence and disconnect handling, delivery/notifications, credits, calendars, access controls, and video integration.

## Suggested message to share

> I created a prototype with mock data covering both the member app and coach dashboard. You can set coach availability, send a member request, accept or decline it, join from both sides, and finish the session with shared next steps. Please try the main flow and the fallback scenarios before I implement it. The review guide explains exactly where to click and what to check. Use the top bar to switch views, or open two tabs in the same browser. Each reviewer has their own demo data.

Only the sanitized static prototype and this walkthrough are published. Private source captures, live application source, credentials, and real account data are excluded.
