<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Monero Privacy Practices</title>
<style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
    }
    h1, h2 {
      color: #2c3e50;
    }
    ul {
      margin-left: 20px;
    }
    p {
      margin-bottom: 10px;
    }
    a {
      color: #2980b9;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
</style>
</head>
<body>
  <h1>Monero Privacy Practices</h1>

  <p>Monero is a cryptocurrency that offers robust privacy features by default,
    but to achieve optimal anonymity, users should follow advanced privacy
    practices.</p>

  <h2>Using Separate Monero Accounts</h2>

  <p>For enhanced privacy, it is recommended to organize your Monero funds
    into separate accounts based on different purposes, such as:</p>

  <ul>
    <li><strong>Work:</strong> For income related to your hard work.</li>
    <li><strong>Cash:</strong> For everyday transactions like groceries.</li>
    <li><strong>Trading:</strong> For funds used in investment activities.</li>
    <li><strong>Mining:</strong> For rewards earned from mining.</li>
    <li><strong>Donations:</strong> For accepting donations.</li>
  </ul>

  <p>When you need to combine funds from these different accounts, avoid sweeping
    or withdrawing balances from multiple accounts in a single transaction.
    Instead, perform one transaction per account to avoid linking them
    together.</p>
  <p>The <a href="https://docs.featherwallet.org/guides/features" target="_blank">Feather Wallet</a>
    offers "Coin control" functions that allow for more granular management
    of your funds, supporting this approach to privacy.</p>

  <h2>Waiting/Aging Monero After Receiving It</h2>

  <p>After receiving Monero (XMR) from a third party, consider waiting some
    time before spending it. This waiting period, which can range from
    a few hours to a few days, helps obscure the link between the incoming
    and outgoing transactions. This practice is particularly useful in
    preventing timing analysis, where an observer might try to correlate
    the time of your transactions with other events.</p>

  <h2>Churning/Mixing Monero by Sending It to Another Own Account</h2>

  <p>Churning or mixing refers to the process of sending your Monero to another
    account or wallet you control to make it harder for others to track
    the origin of your funds. This method leverages Monero's ring signatures
    to re-mix transactions and increase anonymity.</p>
  <p>For example, after one churn, there is a 1 in 16 chance (6.25%) that
    the transaction can be attributed to you. After two churns, the probability
    decreases to 1 in 256 (0.39%), and after three churns, it drops to
    1 in 4096 (0.0244%).</p>

  <h3>A) Sending to a Different Account/Wallet</h3>

  <p>One effective strategy is to send your entire (or part of) account’s
    balance to a different account or wallet you control. This "secret
    destination" account should not be used for receiving funds from third
    parties—only from your own accounts. If you manage multiple Monero
    accounts for different purposes (e.g., "work", "home"), you may want
    to churn each account’s funds multiple times before merging them.</p>

  <h3>B) Sending to the Same Account (Self-Churning)</h3>

  <p>Another method is to send your entire account’s balance back to the same
    account (self-churning). When doing this, avoid sending partial amounts,
    as mixing churned outputs with non-churned ones can reduce the effectiveness
    of this privacy measure. Sending Monero back to the same account is
    effective in enhancing privacy because each transaction creates a new
    set of ring signatures.</p>

  <h2>Waiting/Aging Churned/Mixed Monero Again</h2>

  <p>After churning or mixing your Monero, it is advisable to wait again before
    using the funds. This additional waiting period further complicates
    the transaction history, making it more difficult for an observer to
    establish links between transactions.</p>

</body>
</html>