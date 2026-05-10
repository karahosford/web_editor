---
marp: true
theme: default
transition: fade
class:
---

<style>


h1,
h2,
h3 {
	color: #003c69;
}

</style>

# AI and the Future of the UCC Website
Dr. Kara Hosford

![bg opacity:0.2 blur:4px 160%](images/network.gif)

<!--
Narrator's Notes: 
Welcome everyone. Today, we are going to explore the intersection of artificial intelligence and higher education digital strategies, specifically focusing on the future of the University College Cork (UCC) website. As the digital landscape evolves, so must our approach to engaging students, managing content, and ensuring our platforms are accessible and future-ready. Let's dive into how AI will reshape the UCC digital experience.
-->

---

# Understanding AI Usage Context

### AI is viewed as an enabling tool
The public generally accepts AI-generated media as a pragmatic solution for grassroots organizations to produce high volumes of advocacy content on limited budgets (Dey, 2023).

### UCC's international reach requires a nuanced approach
Cultural values shape trust and adoption, meaning AI integration faces varying levels of acceptance or resistance depending on regional context (AbuDaabes, 2025).

![bg opacity:0.1](images/bg.png)

---

# Current Challenges

Today, users struggle to find the right information quickly and confidently.

**Key barriers on the current site:**
- Accessibility gaps (WCAG 2.1 AA): missing alt text, uncaptioned videos, inaccessible documents
- Important content spread across disconnected pages and sections
- High effort required to move from general interest to the exact answer a user needs

![bg opacity:0.1](images/bg.png)

---

# Current Challenges: *Why This Persists*

- Page publishers are operating under **time pressure** and competing priorities
- Legacy structures were built for **publishing pages**, not for answering user intent
- Navigation remains **hierarchy-first**, while user behavior is increasingly question-first
- As a result, users must **manually connect** information that should already be connected

![bg opacity:0.1](images/bg.png)

---

# From Structure to Discovery: AI Search for UCC

The existing site is like an onion. The future site should behave like a starburst.

**Problem:** The onion model (layered templates and silos) forces users to peel through multiple levels.

**AI Search Solution:** Use AI-driven metadata, relationship mapping, and editorial tagging to surface connected answers in one place. Current web-technologies see user entering natural-language queries expecting to receive a dynamic, connected pathway of relevant content.

![bg right:33%](images/pages.png)

---

<!-- _paginate: false -->
<style scoped>
section {
	padding: 0;
}

.sim-embed {
	width: 100%;
	height: 100%;
	border: 0;
	display: block;
}
</style>

<iframe
	id="ck113-sim-frame"
	src="about:blank"
	data-src="./html/sim.html"
	loading="lazy"
	title="CK113 AI search simulation"
	class="sim-embed"
></iframe>

<script>
(() => {
	const frame = document.getElementById("ck113-sim-frame");
	if (!frame) return;

	const loadFrame = () => {
		if (frame.src === "about:blank") {
			frame.src = frame.dataset.src;
		}
	};

	if ("IntersectionObserver" in window) {
		const observer = new IntersectionObserver(
			(entries) => {
				for (const entry of entries) {
					if (entry.isIntersecting) {
						loadFrame();
						observer.disconnect();
						break;
					}
				}
			},
			{ threshold: 0.6 }
		);

		observer.observe(frame);
	} else {
		// Fallback for environments without IntersectionObserver.
		loadFrame();
	}
})();
</script>

<!--
An accessible familiar interface to answer questions.

The content is there, the website is fine. It's about taking what's there and making it accessible.

We're not reinventing the wheel, the car is in motion. But I'd rather have Google maps to help me than an old map book.

But something like this wouldn't happen over-night.. 

-->

---

# Ai isn't the Bandaid Soloution

1. **Maintain HTML-first publishing** across units, with accessible Word/PDF only where necessary
2. **Apply consistent metadata and taxonomy** so pages are discoverable, linkable, and interpretable
3. **Embed accessibility standards in authoring**: headings, lists, tables, alt text, captions/transcripts, and plain language
4. **Support moderators through training and guidance** so standards are applied consistently in day-to-day publishing
5. **Review and improve continuously** to strengthen quality, compliance, and search reliability over time

![bg opacity:0.1](images/bg.png)

---

# What This Means for the Web Content Editor Role

- **Operationalize standards:** turn accessibility and content rules into repeatable editorial workflows
- **Use AI with oversight:** apply AI to support tasks (alt text suggestions, transcript workflows, readability checks) with human sign-off
- **Improve discoverability:** strengthen metadata quality, internal linking, and taxonomy consistency across content types
- **Enable inclusive reach:** support multilingual and plain-language content for diverse audiences
- **Protect quality and brand:** maintain institutional voice, editorial accuracy, and governance accountability

<!--
Narrator's Notes: 
Accessibility is not optional; it's essential for an equitable experience. Currently, our accessibility statement notes that our site is only partially compliant with WCAG 2.1 Level AA guidelines, with gaps like missing alt text and uncaptioned videos. This is where AI becomes a game-changer. AI can streamline our compliance by automatically generating alt text, creating video transcripts, and checking readability at scale. It can even help with language translation for our international audiences, allowing us to provide an inclusive digital environment without overwhelming our staff.
-->

![bg opacity:0.1](images/bg.png)

---

# Why This Approach Works for UCC

- AI should **augment** staff capability, not replace professional judgment
- UCC retains full editorial and governance **control**
- Human context remains essential for **quality**, **trust**, and **inclusivity**
- Institutional voice and brand **integrity** remains protected

![bg right:40%](images/ucc_01.jpg)

---

# How I Would Deliver in This Role

- Build and maintain an editorial workflow that balances **speed, quality, and compliance**
- Use trusted AI to support repetitive tasks (alt text, summaries, metadata) while keeping **human sign-off**
- Prioritize **student-centered** journeys so users move from query to answer quickly
- Measure impact through **accessibility compliance**, engagement metrics, and content performance
- **Collaborate** across schools and services to keep the UCC voice consistent and trusted

![bg opacity:0.1](images/bg.png)

---

# Thank You

## References

Dey, Neelam C. "'Unleashing the Power of Artificial Intelligence in Social Work: A New Frontier of Innovation'." Available at SSRN 4549622 (2023).

AbuDaabes, Ajayeb Salama, Hany Mamdouh Selim, and Rawa Hijazi. "From clicks to campus: how AI-powered digital marketing shapes student enrollment decisions." Asia-Pacific Journal of Business Administration (2025): 1-20.

![bg opacity:0.1](images/bg.png)