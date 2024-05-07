# Isabelle Proof Scripts for the Secrecy in the SET Payment Protocol

## Summary
These proof scripts are originally distributed at http://www.brl.ntt.co.jp/people/sakurada/set-secrecy/ as
the supplementary material for the paper:
    Hideki Sakurada,
    Verification of Secrecy of the SET Payment Protocol (in Japanese),
    IPSJ Journal, Vol.44, No.8, pp.2106-2116, 2003
    http://id.nii.ac.jp/1001/00011162/

These proof scripts verify the secrecy of PAN(Primary Account Number), in the SET Payment Protocol. These are tested on Isabelle99-1.

## Caution!
This patch modifies some of the scripts distributed with Isabelle. It may break the other part of Isabelle.

## Usage
1. Extract Isabelle99-1 distribution in some directory and build it.
% tar xzvf Isabelle99-1.tgz
% ...
	
2. Change directory into Isabelle99-1/src/HOL/Auth.
% cd Isabelle99-1/src/HOL/Auth
	
3. Process the auth.diff file with patch command.
% patch -p1 < auth.diff
	
4. Verify proofs with Isabelle.
% ../../../bin/isabelle
...(misc. messages from your ML runtime)...
> use_thy "SPT";
