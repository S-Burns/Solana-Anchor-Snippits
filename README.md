# Solana-Anchor-Snippits
Snippet Collection of Anchor Code for cut and paste creation applications on Solana using programs(aka Smart Contracts) and querying the Solana network.

If you want to learn *how* anchor works, use https://book.anchor-lang.com/. If you want the cut and paste of what to do, you are in the right place:

*Note: Version mismatch of code incompatability is the norm in Anchor givent the current state. Thus install and mind the AVM 
**Overview: Currently the '/program/lib.rs' contains virtually all proprietary business logic of what is classically considered the backend or serverside code and the '/app/' folder contains all propreitary business logic on the frontend; thus all changes exist in these folders, save for the version recorded in the 'Cargo.toml' under the 'program' folder.

Precursors:
1. Using Windows Subsystem Linux or WSL is essentially an imparitive. https://docs.microsoft.com/en-us/windows/wsl/install
2. Using the Anchor Version Manager aka AVM is highly recommended. Install and use details here https://book.anchor-lang.com/chapter_4/avm.html.
3. Always use a unique Program_ID contained in declare_id!("<UNIQUE_Program_ID>") that will be generated on your local machine following these instructions..

Program(aka Smart Contract) Use Cases:
1. Blog - Solblog_lib.rs Main program rust file 
2. Poll - poll_lib.rs Main program rust file 

Query Use Cases:
1. SQL queries on  https://dune.xyz/queries Dune_SQL 
