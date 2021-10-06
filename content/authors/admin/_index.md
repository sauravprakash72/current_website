---
# Display name
# title: Saurav Prakash

# Is this the primary user of the site?
superuser: true

# Role/position/tagline
role: PhD Candidate in Electrical and Computer Engineering

# Organizations/Affiliations to show in About widget
organizations:
- name: University of Southern California
  url: https://www.usc.edu/ 

# Short bio (displayed in user profile at end of posts)
bio: I am a graduate student with interests in privacy-preserving, secure, and distributed data analytics.

# Interests to show in About widget
interests:
- Secure and Privacy-Preserving Machine Learning
- Federated Learning 
- Large-Scale Serverless Training 
- Coded Distributed Computing 
- Information and Coding Theory

# Education to show in About widget
education:
  courses:
  - course: PhD in Electrical and Computer Engineering
    institution: University of Southern California
    year: 2022 (expected)
  - course: BTech in Electrical Engineering
    institution: Indian Institute of Technology Kanpur
    year: 2016

# Social/Academic Networking
# For available icons, see: https://wowchemy.com/docs/getting-started/page-builder/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "/#contact" for contact widget.
social:
- icon: google-scholar  # Alternatively, use `google-scholar` icon from `ai` icon pack
  icon_pack: ai
  link: https://scholar.google.com/citations?user=VhnTrugAAAAJ&hl=en
- icon: researchgate  
  icon_pack: ai
  link: https://www.researchgate.net/profile/Saurav-Prakash-2
- icon: semantic-scholar  
  icon_pack: ai
  link: https://www.semanticscholar.org/author/Saurav-Prakash/47592370
- icon: linkedin
  icon_pack: fab
  link: https://www.linkedin.com/in/saurav-prakash-38504264/
- icon: envelope
  icon_pack: fas
  link: "mailto:sauravpr@usc.edu"

# Link to a PDF of your resume/CV.
# To use: copy your resume to `static/uploads/resume.pdf`, enable `ai` icons in `params.toml`, 
# and uncomment the lines below.
# - icon: cv
#   icon_pack: ai
#   link: uploads/resume.pdf

# Enter email to display Gravatar (if Gravatar enabled in Config)
email: "sauravpr@usc.edu"

# Highlight the author in author lists? (true/false)
highlight_name: false
---

Hi, I am a PhD candidate in the <a href="https://minghsiehece.usc.edu/">Ming Hsieh Department of Electrical and Computer Engineering</a> at the <a href="https://www.usc.edu/"> University of Southern California</a>, working under the guidance of <a href="https://www.avestimehr.com/">Prof. Salman Avestimehr</a> in the <a href="https://www.avestimehr.com/vital-lab">Information Theory and Machine Learning (vITAL)</a> research lab. During my research pursuits, I have also collaborated closely with <a href="https://annavar.am/">Prof. Murali Annavaram</a>, <a href="https://hal.usc.edu/chugg/">Prof. Keith Chugg</a>, and <a href="https://web.ece.ucsb.edu/~ramtin/">Prof. Ramtin Pedarsani</a>. I have also had the fortune to gain industry experience through multiple internships. I spent Summer 2018 and Summer 2019 as a Research Intern at Intel Labs under <a href="https://scholar.google.com/citations?user=plidYfUAAAAJ">Dr. Shilpa Talwar</a> and <a href="https://scholar.google.com/citations?hl=en&user=frmNZH4AAAAJ">Dr. Nageen Himayat</a> respectively. During Summer 2021, I was an Applied Scientist Intern at Amazon Alexa AI under <a href="https://scholar.google.com/citations?hl=en&user=wBkmDegAAAAJ">Dr. Clement Chung</a> and <a href="https://guptarah.github.io/">Dr. Rahul Gupta</a>. Prior to joining the graduate school, I completed my BTech in 2016 in <a href="https://www.iitk.ac.in/ee/">Electrical Engineering</a> from the <a href="https://iitk.ac.in/">Indian Institute of Technology Kanpur</a>, where I worked under <a href="http://home.iitk.ac.in/~adityaj/">Prof. Aditya K. Jagannatham</a>, in the <a href="http://www.iitk.ac.in/mwn/">Multimedia Wireless Networks (MWN)</a> Group.


As a graduate student, I have been working towards holistically addressing real-world bottlenecks in large-scale distributed computing, including federated learning. My <a href='#projects'>projects</a> are broadly classified into the following three exciting paradigms:
<!-- <ol>
  <li><em>Server-assisted computing with centralized data placement:</em> In this domain, a crucial problem that I have focused on is that of the large-scale machine learning in sevrer farms, where server entity has full control over data. In this setting, one of the key bottlenecks is that of straggling nodes, that can degrade the  training performance significantly by slowing it down. </li>
  <li><em>Server-assisted computing with data at the edge users:</em> This includes the problem of federated learning, where a server entity, such as Google, wants to train a machine learning model from data at the users, while ensuring data privacy. Two key bottlenecks that I have addressed in my research works are mititgation of stragglers, and mitigation of nodes causing Byzantine (arbitrary) errors during the training process, both of them being for the general heterogeneous data distribution across the nodes. </li>
  <li><em>Decentralized (serverless) computing:</em> Problems in serverless computing include consensus based optimization, where a group of nodes want to learn a model over data available across the entirety of the nodes. There is no central authority to orchestrate the process in this setting. My recent work in this domain addresses Byzantine mitigation, which is quite challenging due to the absence of a central trusted coordinator.</li>
</ol> -->
<ol>
  <li><b>Privacy-Preserving and Robust Machine Learning at the Edge:</b> In many machine learning applications, private training data is distributed across multiple users, such as patient records at multiple hospitals, giving rise to the following multi-dimensional problem: How can individual users jointly train an ML model while (1) keeping their individual datasets private; (2) exploiting the heterogeneity of data across users; and (3) being resilient against straggling and malicious users. For example, a key difficulty in mitigating malicious users when data is non-IID across users is that even the updates from non-malicious users are quite diverse, hence prior outlier based strategies perform poorly. My focus has been to resolve this conundrum both in the federated learning setting (where a central server orchestrates the training), as well as in the serverless decentralized training setting.    
  </li>
  <li><b>Efficient Large-Scale Distributed Learning in the Cloud:</b> In large-scale training tasks, such as pre-training of NLP models with billions of parameters (e.g., GPT-3), straggling nodes adversely impact the performance by increasing the tail latency. A simple way herein is to ignore the computations carried out at the straggling nodes. However, in many industry settings, ignoring straggling tasks is not favored as it reduces the model quality. This is very critical since the model will be used by millions of people and even a slight improvement is quite remarkable in practice. My focus in this domain has been to leverage novel computation redundancy for making distributed training straggler-resilient, leading to a significant improvement in the overall training time while simultaneously preserving the optimal convergence performance. </li>
  <li><b>Foundations of Coded Computing:</b> Coded computing is a nascent transformative framework for injecting computation redundancy in unorthodox encoded forms in order to efficiently deal with communication bottleneck and system disturbances including stragglers, system and statistical heterogeneity, and adversarial computations in distributed systems. Two of the key research problems where I have leveraged as well as advanced the coded computing domain are (1) communication efficient large-scale graph processing, and (2) low-latency federated learning in wireless edge networks.  
  </li>
</ol>


Outside research, I like hanging out with friends, watching classical Bollywood movies, and listening to Indian classical music. 

