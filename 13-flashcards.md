# Flashcards - SC-300

> Click any card to reveal the answer. Use the Domain pager bottom-right to switch between exam areas.

<section class="fc-section" data-fc-title="Implement Identities in Microsoft Entra">
<h2>1 - Implement Identities in Microsoft Entra</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Three hybrid auth methods?</div><div class="fc-a">PHS, PTA, Federation (AD FS).</div></div>

<div class="flashcard"><div class="fc-q">Most lightweight hybrid sync engine?</div><div class="fc-a">Microsoft Entra Cloud Sync (agent-only, no SQL).</div></div>

<div class="flashcard"><div class="fc-q">What is an Administrative Unit?</div><div class="fc-a">A scoped container for delegated admin (e.g. all users in a region).</div></div>

<div class="flashcard"><div class="fc-q">Where do you onboard partner users?</div><div class="fc-a">Microsoft Entra External ID -> B2B (guest) collaboration, ideally via entitlement management.</div></div>

<div class="flashcard"><div class="fc-q">Difference between assigned and dynamic groups?</div><div class="fc-a">Assigned = manually managed members. Dynamic = membership rule (e.g. department eq 'Sales'). Dynamic requires P1.</div></div>

</div>
</section>
<section class="fc-section" data-fc-title="Implement Authentication and Access Management">
<h2>2 - Implement Authentication and Access Management</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Most impactful single CA policy?</div><div class="fc-a">Block legacy authentication.</div></div>

<div class="flashcard"><div class="fc-q">Authentication strength examples?</div><div class="fc-a">MFA, Passwordless MFA, Phishing-resistant MFA - assignable in CA grant control.</div></div>

<div class="flashcard"><div class="fc-q">User risk vs sign-in risk?</div><div class="fc-a">User risk = compromised credentials over time. Sign-in risk = anomalous individual sign-in event.</div></div>

<div class="flashcard"><div class="fc-q">What is CAE?</div><div class="fc-a">Continuous Access Evaluation - token revocation events pushed to clients/RPs near-real-time.</div></div>

<div class="flashcard"><div class="fc-q">How do you onboard a passwordless user?</div><div class="fc-a">Issue a Temporary Access Pass (TAP), have them register passkey/FIDO2/WHfB.</div></div>

<div class="flashcard"><div class="fc-q">What licenses does Identity Protection require?</div><div class="fc-a">Entra ID P2 (or M365 E5).</div></div>

</div>
</section>
<section class="fc-section" data-fc-title="Plan and Implement Workload Identities">
<h2>3 - Plan and Implement Workload Identities</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">App registration vs service principal?</div><div class="fc-a">Registration = the app definition (single object in home tenant). SP = the runtime instance (one per tenant the app is consented in).</div></div>

<div class="flashcard"><div class="fc-q">System-assigned vs user-assigned MI?</div><div class="fc-a">System = 1:1 with resource, deleted when resource deleted. User-assigned = standalone, sharable.</div></div>

<div class="flashcard"><div class="fc-q">Best OAuth flow for SPA?</div><div class="fc-a">Auth code with PKCE.</div></div>

<div class="flashcard"><div class="fc-q">OAuth flow for daemon?</div><div class="fc-a">Client credentials with certificate (or secret).</div></div>

<div class="flashcard"><div class="fc-q">What is OBO?</div><div class="fc-a">On-Behalf-Of - token exchange so an API can call a downstream API as the user.</div></div>

<div class="flashcard"><div class="fc-q">What does Application Proxy provide?</div><div class="fc-a">Reverse proxy for on-prem web apps with Entra ID auth, no VPN.</div></div>

<div class="flashcard"><div class="fc-q">How do you apply CA to a service principal?</div><div class="fc-a">Workload Identities P2 license + CA policy with workload ID assignment.</div></div>

</div>
</section>
<section class="fc-section" data-fc-title="Plan and Implement Identity Governance">
<h2>4 - Plan and Implement Identity Governance</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">What is an access package?</div><div class="fc-a">Bundle of resources (groups, apps, sites) granted via self-service request + approval + lifecycle in entitlement management.</div></div>

<div class="flashcard"><div class="fc-q">PIM eligible vs active assignment?</div><div class="fc-a">Eligible = must activate (MFA, justification). Active = always-on.</div></div>

<div class="flashcard"><div class="fc-q">How do you certify privileged role membership?</div><div class="fc-a">Access review campaign on PIM-eligible role assignments.</div></div>

<div class="flashcard"><div class="fc-q">Lifecycle workflows automate what?</div><div class="fc-a">Joiner-mover-leaver tasks (welcome email, group adds, account disable, group removes, etc.).</div></div>

<div class="flashcard"><div class="fc-q">How long are Entra sign-in logs free?</div><div class="fc-a">30 days in the portal. Longer requires Log Analytics / Sentinel ingestion.</div></div>

</div>
</section>

---

[Master Index](00-MASTER-INDEX.md)
