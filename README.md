### Hi, I'm Hari Kheshav. These projects are built by AI agents 🤖

Every project on this account was written end-to-end by AI coding agents (mostly
[Claude Code](https://www.anthropic.com/claude-code)): the code, tests and documentation.
My part: the idea and the goals, design direction, reviewing the results, and bringing
things up on real hardware.

My own work lives on my main account: **[@Harikheshav](https://github.com/Harikheshav)**.

#### Projects

| Project | What it is | Website |
|---|---|---|
| [RV32I-SOC](https://github.com/harikheshav-ai/RV32I-SOC) | Pipelined RV32I core in Bluespec with a UART-loaded SoC, co-simulated against Spike and running on an Arty A7-100T via an open-source FPGA flow | [site](https://harikheshav-ai.github.io/RV32I-SOC/) |
| [tinyllm_fpga](https://github.com/harikheshav-ai/tinyllm_fpga) | llama2.c stories15M on a custom int8 GEMV accelerator, verified bit-exact on a VC707 (13 tok/s) | [site](https://harikheshav-ai.github.io/tinyllm_fpga/) |
| [ros2-shakti](https://github.com/harikheshav-ai/ros2-shakti) | ROS 2 Jazzy (155 packages, Cyclone DDS, `ros2` CLI) cross-built for the Shakti C-Class RISC-V core under Linux 6.6, tested in QEMU | – |

A few more experiments are private for now.

#### How to read these repos
- Each README starts with a note on how it was made and what my role was.
- Results are checked, not just generated: simulations against reference models, and hardware runs where noted.
- Some repos include a session analysis of how the agent worked, including its mistakes.

#### How this account is managed (by Claude)
Claude Code also handles the GitHub side of these projects, under a few rules:
- **Separate identity.** A dedicated account, its own SSH key and a no-reply commit email, so AI-built work never
  counts toward my main account.
- **Approval first.** Claude prepares everything locally and asks before every push which account to use;
  public or private is always my call.
- **Only sources in git.** Build outputs, model weights and datasets are kept out with `.gitignore`; large
  artefacts (weights, bitstreams, generated data) are published as releases with checksums.
- **Upstream respected.** Third-party code stays as pinned upstream commits or patch files, with its licences.
- **Checked before publishing.** Every file is scanned for local paths, personal names and credentials, and
  session logs are redacted.
- **Reproducibility checks.** Independent agents clone each repo fresh and follow only its README; anything that
  breaks is fixed and re-tested before it is pushed.
