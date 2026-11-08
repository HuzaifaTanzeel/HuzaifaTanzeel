<h1 align="center">Huzaifa Tanzeel</h1>

<p align="center">
  <b>Backend engineer. AI engineer. DevOps engineer.</b><br/>
  Mostly I'm the person who connects the three.
</p>

<p align="center">
  <a href="mailto:hthuzaifatanzeel@gmail.com">Email</a> ·
  <a href="https://linkedin.com/in/huzaifatanzeel">LinkedIn</a> ·
  <a href="https://medium.com/@hthuzaifatanzeel">Medium</a>
</p>

---

Picture a real Android phone, not an emulator, working its way through a mobile app. Nobody is touching it. An AI agent is reading the screen, deciding what to tap, and moving on.

Now picture everything that has to be true for that to work. The backend services behind it have to stay up. The phone has to be online, charged, and not wedged in some strange state. The servers it talks to have to be deployed the same way every time. And when something breaks at 3 a.m., a dashboard has to say which part broke.

That chain is where I spend my time. I'm a polymath by habit, not by plan: every time I solved one problem, the next one was sitting one layer down the stack, so I went and learned that layer too.

---

## Chapter 1: Services that have to stay up

<img src="assets/sofy-logo.png" alt="Sofy.ai" height="36"/>

My first real job was backend work at [Sofy.ai](https://sofy.ai), on a platform built from distributed Java and Spring Boot services. Plenty of people were using it at once, so I got used to thinking in terms of what happens when two customers want the same thing at the same moment, and what a slow database does to everyone else.

Redis ended up solving a lot of that for me: locking devices so two customers could never be handed the same one, and caching hot API responses to take load off the database.

## Chapter 2: An agent with real hands

Then the problem got more interesting. I designed an AI testing agent that drives **real Android devices** through Appium, not simulators. It walks the UI flows of enterprise mobile apps, the kind of apps where a bug is expensive. It was used to test flows for companies like **SAP** and **Careem**.

Real hardware is stubborn. Screens lag, permissions pop up, a GPS location needs faking, a button is only visible in the OCR output. Most of the engineering was in making an agent calm enough to deal with all of that.

## Chapter 3: Keeping the fleet alive

An agent is only as reliable as the phones under it, so I ended up owning that part too.

I deployed services across multiple servers with **Ansible playbooks**, and built the observability layer with **Prometheus, Loki, and Grafana** to watch both the infrastructure and the devices themselves. The goal was boring on purpose: real Android and iOS hardware staying stable and available on the portal. Better monitoring cut manual debugging effort by about 90%.

## Chapter 4: RAG, voice, and ten VMs at once

<img src="assets/acs-logo.png" alt="Arabic Computer Solutions" height="64"/>

At [Arabic Computer Solutions](https://arabic-computer.com) the story continued on the AI side. I worked on **RAG systems** and **voice AI** capabilities, and on the Linux servers that run them.

Java and Spring Boot services get dockerized and released through an on-prem GitLab. Ansible playbooks then carry each release out to **10+ VMs at a time**, so a deployment is one command instead of an afternoon.

---

## A side quest I'm proud of

**An AI avatar that gives a resort tour.** A guest talks to a live, lip-synced avatar while moving through a 360° virtual tour of the InterContinental Maldives. Ask to see the overwater villa and the tour takes you there. The brochure, the navigation, and the follow-up email are all things the agent can do, not just talk about.

I built it independently with FastAPI, RAG, PostgreSQL, Docker Compose, and real-time orchestration between the agent and the tour.

[![AI Avatar Video Agent for InterContinental Maldives](https://img.youtube.com/vi/s9f5Tx7cSPc/maxresdefault.jpg)](https://youtu.be/s9f5Tx7cSPc)

---

## The toolbox

**Backend and AI:** Python, FastAPI, Java, Spring Boot, PostgreSQL, RAG, voice agents

**Devices:** Appium on physical Android hardware, plus the iOS devices on the same portal

**Delivery and observability:** Docker, Linux, Ansible, on-prem GitLab, Prometheus, Grafana, Loki, Kubernetes

<p>
  <img src="https://skillicons.dev/icons?i=py,fastapi,java,spring,postgres,docker,linux,ansible,gitlab,prometheus,grafana,kubernetes,git,github&perline=7" />
</p>

## Things I've written

- [Understanding WebRTC: A Beginner's Guide to Real-Time Communication](https://medium.com/@hthuzaifatanzeel/understanding-webrtc-a-beginners-guide-to-real-time-communication-on-the-web-2fbe75f7a8e1)
- [Kubernetes Basics: Components & Architecture](https://medium.com/@hthuzaifatanzeel/kubernetes-basics-components-architecture-5af7345543dc)
- [Minikube & Kubectl: Local Setup Guide](https://medium.com/@hthuzaifatanzeel/minikube-kubectl-local-setup-856497eaa135)

## Beyond the day job

Open source contributor to [Awesome LLM Apps](https://github.com/Shubhamsaboo/awesome-llm-apps) and Appium Device Farm. Invited panel speaker at HackFest 2026 (IBA) on agentic systems, and technical mentor at HackOps 2025 (FAST-NUCES Karachi), where I presented on observability.

BS Computer Science, FAST NUCES Karachi.

---

<p align="center"><i>If you have a problem that spans the stack, I'd like to hear about it.</i></p>
