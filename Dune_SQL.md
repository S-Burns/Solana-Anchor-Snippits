Precursor:
1. Create Account https://dune.xyz/
2. Navigate to https://dune.xyz/queries/ and Select the "Solana" network

Query... 

1. Solana.blocks = The full block history for the Solana ecosystem 
'
SELECT date_trunc('day', time), count(*) FROM solana.blocks WHERE time IS NOT NULL GROUP BY 1;
'

2. Solana.transactions = The data for transactions including programs called and account activity 
'
select 
    date,
    count(*) AS TPD
FROM solana.blocks
WHERE date is not null
GROUP BY 1
'

3. Solana.rewards =The rewards paid out on Solana

'
select reward_type as reward_type, count(*) as count from solana."rewards" group by reward_type order by count
'
