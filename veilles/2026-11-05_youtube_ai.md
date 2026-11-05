# Veille YouTube IA – 5 novembre 2026

**Période couverte :** ~2-5 novembre 2026  
**Focus :** Anthropic (priorité 1) > IA locale > IA chinoises > IA françaises  
**Critères :** technique/avancé (code, architectures, papers) · nouveauté + clarté + profondeur · FR/EN/ZH (sous-titres OK) · top 8-10 si flux riche · officiels secondaires

---

## 1. Anthropic – Comment ils merge 30 000 changements de code par jour
**Lien :** https://www.youtube.com/watch?v=AnsXWH2_EBU  
**Chaîne :** AI Engineer · ~19 min · ~87k vues · 28-29 oct. 2026  
**Tags :** #Anthropic #ClaudeCode #SoftwareFactory #CodeReview #Agents

**Points clés :**
- Anthropic est passé de ~2 500 à 30 000 merges/jour grâce à Claude en first-pass review + vérification multi-couches (tests, sandboxes, preuves).
- Distinction « light vs dark software factories » : le goulot n’est plus le coding mais la confiance/qualité.
- Données Sonar State of Code + retours Addy Osmani (Anthropic) et Manish Kapur (Sonar).
- Lightning round sur le labeling des PRs agents et critères de merge safe.

**Pourquoi la regarder :** Vision concrète et très technique de l’usine logicielle interne d’Anthropic à l’ère des coding agents. Directement actionnable pour toute équipe qui scale Claude Code / agents.

---

## 2. Anthropic – Architecture « brain and the hands » (Managed Agents)
**Lien :** https://www.youtube.com/watch?v=MRQTlwcW-aQ  
**Chaîne :** Latent Space · ~1h47 · 27 oct. 2026  
**Tags :** #Anthropic #ManagedAgents #AgentArchitecture #ClaudeOpus5.5 #Sandboxes

**Points clés :**
- Conversation avec les heads of Engineering & Product d’Anthropic (Katelyn Lesse, Angela Jiang).
- Séparation claire : brain (modèle) / hands (exécution) – sandbox qui peut mourir sans tuer l’agent.
- Credentials isolés, Messages API réécrit en Rust avec Claude + shadow traffic, protection contre distillation.
- Opus 5.5 positionné comme daily driver enterprise pour agents long-running.

**Pourquoi la regarder :** Deep dive rare sur l’architecture production d’Anthropic. Très dense et technique.

---

## 3. Claude Desktop « v2 » – rebuild complet (artifacts, Code tab, multitasking)
**Lien :** https://www.youtube.com/watch?v=tM0dwXhOv2o  
**Chaîne :** Futurepedia · ~15 min · 3 nov. 2026  
**Tags :** #Claude #DesktopApp #ClaudeCode #Artifacts #Productivity

**Points clés :**
- Rebuild majeur de l’app desktop (certains ingénieurs le considèrent comme un vrai Claude 2.0).
- Nouveaux formats d’artifacts (docs, slides, design, dashboards, motion).
- Session rail, context breakdown, side chats, split view, remote control, cloud sessions, nested sessions, task chips.
- Mods et setup kit fournis.

**Pourquoi la regarder :** Meilleure vue d’ensemble pratique des nouvelles capacités productives de Claude (Code + artifacts) pour usage quotidien avancé.

---

## 4. Nouveau workflow Claude Code : skills, hooks, review loops
**Lien :** https://www.youtube.com/watch?v=S49gppZl8H0  
**Chaîne :** AI LABS · ~16 min · 30 oct. 2026  
**Tags :** #ClaudeCode #Skills #Hooks #Evals #AgentWorkflow

**Points clés :**
- Comment l’équipe Claude Code d’Anthropic vérifie le travail des agents (écriture d’evals + design mock + hooks bloquants).
- REVIEW.md + CLAUDE.md pour imposer les règles de revue.
- Boucle builder → verifier → reviewer jusqu’à passage des evals.
- Résultats internes : + de changements, –40 % de rollbacks.

**Pourquoi la regarder :** Pattern concret et copiable pour rendre les coding agents fiables en production.

---

## 5. IA locale – Quel runtime choisir en 2026 (Ollama vs LM Studio vs llama.cpp vs vLLM)
**Lien :** https://www.youtube.com/watch?v=Dvg9QfWkqKE  
**Chaîne :** ErrorFixer · ~4 min · fin sept./oct. 2026 (toujours très pertinent)  
**Tags :** #LocalAI #Ollama #LMStudio #llama.cpp #vLLM

**Points clés :**
- Trois tiers : desktop apps / single-user servers / high-throughput engines.
- Comparaison install, API quirks, concurrence, hardware.
- Scorecard de compatibilité et « breakage clinic ».

**Complément récent :**  
- llama.cpp v0.8.0 ajoute realtime voice chat + TTS (https://www.youtube.com/watch?v=LxPloFHz4BY)  
- Guide mémoire 16–128 Go (chinois, sous-titres) : https://www.youtube.com/watch?v=1nomxygMILI (4 nov.)

**Pourquoi les regarder :** Décision claire et à jour pour setup local technique.

---

## 6. Kimi K3.1 Pro (Moonshot) – Open weights presque au niveau Opus
**Lien :** https://www.youtube.com/watch?v=zgluzf-zjhI  
**Chaîne :** Prompt Engineering · ~1 min (teaser) + analyses détaillées  
**Analyses recommandées :**  
- https://www.youtube.com/watch?v=9bgM_nJfxZM (Universe of AI, ~9 min)  
- Fireship : https://www.youtube.com/watch?v=G_em1hHPnXY (~6 min, 2.4M vues)  
**Tags :** #Kimi #Moonshot #OpenWeights #ChineseAI #TerminalBench

**Points clés :**
- 2.8T paramètres MoE (~104B active), 1M context, open weights promis pour le 4 nov. (statut à vérifier).
- Terminal-Bench 4.0 : ~65.7 % (vs Opus 5.5 66.4 %, GPT-6 Astra 58 %).
- Pricing API très agressif ($2/$10), suppression des données cyber pour la release open.
- Très fort en coding / agents / 3D.

**Pourquoi la regarder :** Meilleur open-weight chinois actuel, très proche des frontier closed.

---

## 7. DeepSeek – Nouveau Harness + Super Agent (réponse à Claude Code)
**Lien :** https://www.youtube.com/watch?v=OrcsMi2-IcM  
**Chaîne :** Sam Witteveen · ~18 min · 3 nov. 2026  
**Tags :** #DeepSeek #AgentHarness #SuperAgent #OpenSource #CodingAgent

**Points clés :**
- DeepSeek Harness (MIT) + Super Agent add-on : agent qui watch issues/PRs, travaille en session isolée et ouvre des PRs.
- Pas verrouillé aux modèles DeepSeek.
- Web UI + desktop, très actif sur GitHub.

**Pourquoi la regarder :** Alternative open-source concrète et mature aux coding agents fermés.

---

## 8. Mistral Large 4 (open weights) + contexte IA française
**Contexte :** Mistral Large 4 (Le Chonk) open weights annoncés fin octobre 2026.  
**Vidéos à surveiller / analyses :** chercher « Mistral Large 4 » sur YouTube (flux encore en train de se former).  
**Tags :** #Mistral #FrenchAI #OpenWeights

**Note :** Peu de deep-dives techniques ultra-récents au moment de la veille ; à prioriser dans la prochaine (7-9 nov.).

---

## 🚀 Actions prioritaires

1. Regarder en priorité **#1 (30k merges)** et **#2 (Managed Agents architecture)** – vision interne Anthropic.
2. Tester le workflow review loops de **#4** sur un projet Claude Code personnel.
3. Suivre le statut exact des open weights Kimi K3.1 Pro et tester DeepSeek Super Agent.
4. Mettre à jour son setup local avec llama.cpp 0.8+ (voice) et choisir runtime selon hardware.

---

*Veille générée le 5 novembre 2026. Sources principales : AI Engineer, Latent Space, Futurepedia, AI LABS, Prompt Engineering, Universe of AI, Fireship, Sam Witteveen, chaînes techniques locales (llama.cpp / Ollama).*
