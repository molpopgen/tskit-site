---
layout: software-page
title: msprime
name: msprime
#Uncomment to override automatic values
#description: 
#repo_url: 
gh_org: tskit-dev
# TODO change to stable once msprime 1.0 is shipped.
docs_url: https://tskit.dev/msprime/docs/latest
category: simulate
permalink: /msprime
python_package: msprime
logo: https://user-images.githubusercontent.com/8552/101000815-4837ad00-3556-11eb-8597-490e44f53f41.png
code_snippet: |2
  ts = msprime.sim_ancestry(
      samples=10, 
      recombination_rate=1e-4, 
      sequence_length=1e6
  )
  ts = msprime.mutate(ts, rate=1e-6)
---

Msprime is a Python package that simulates ancestral histories and 
DNA sequence data. Msprime uses backwards-in-time "coalescent" models
which allows it to simulate data very efficiently; however, it 
is not as flexible as forwards-in-time simulators like SLiM or fwdpy11.
