<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>crypto</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html"><hr>
<h1 id="crypto-wallet-and-transaction-system-documentation">Crypto Wallet and Transaction System Documentation</h1>
<p>This documentation provides a clear, user-friendly breakdown of the cryptocurrency platform’s functionality. It explains how users create and manage wallets, make transactions, and buy tokens directly within the app. The guide will help your design and development teams align on both user experience and technical requirements for the platform.</p>
<hr>
<h2 id="overview">Overview</h2>
<p>This system allows users to create crypto wallets, perform transactions using a secure and straightforward process, and even buy cryptocurrency directly through the app. It is designed for accessibility, enabling users to manage their crypto easily, with robust security measures in place for data protection and transaction integrity.</p>
<p>Users register with essential details, including a phone number as their unique identifier for transactions and wallet linking.</p>
<hr>
<h2 id="key-user-actions">Key User Actions</h2>
<ol>
<li>
<p><strong>User Registration</strong>: Sign up with username, name, email, password, and phone number (unique identifier).</p>
</li>
<li>
<p><strong>Wallet Creation and Selection</strong>: Users can create wallets for various supported cryptocurrencies, each requiring its own wallet.</p>
</li>
<li>
<p><strong>Secure Transactions</strong>: Users can conduct transactions using a recipient’s phone number, with additional peer-to-peer (P2P) transaction options.</p>
</li>
<li>
<p><strong>Pending Transactions for New Users</strong>: Transactions to non-registered users remain pending until they join the platform.</p>
</li>
<li>
<p><strong>P2P Transactions</strong>: Facilitates direct crypto transfers between registered users.</p>
</li>
<li>
<p><strong>Buying Cryptocurrency Directly</strong>: Users can buy crypto directly from the platform, which purchases it from third-party providers and resells it with a small commission.</p>
</li>
</ol>
<hr>
<h2 id="user-journey-mapping">User Journey Mapping</h2>
<p>Here is a step-by-step guide to the user’s journey, covering each action and illustrating the backend processes involved.</p>
<h3 id="user-registration">1. User Registration</h3>
<ul>
<li>
<p><strong>Inputs Required</strong>:</p>
</li>
<li>
<p>Username</p>
</li>
<li>
<p>First and Last Name</p>
</li>
<li>
<p>Email Address</p>
</li>
<li>
<p>Password</p>
</li>
<li>
<p>Phone Number (serves as the unique identifier for transactions)</p>
</li>
<li>
<p><strong>Process</strong>:</p>
</li>
<li>
<p>Users submit their details.</p>
</li>
<li>
<p>The system verifies the phone number’s uniqueness.</p>
</li>
<li>
<p><strong>Outcome</strong>:</p>
</li>
<li>
<p>Upon successful registration, the user is redirected to their dashboard, ready to set up wallets.</p>
</li>
</ul>
<h3 id="selecting-a-chain-and-adding-wallets">2. Selecting a Chain and Adding Wallets</h3>
<ul>
<li>
<p><strong>Purpose</strong>: Allow users to set up wallets for specific cryptocurrencies like Bitcoin (BTC), Ethereum (ETH), or Tether (USDT).</p>
</li>
<li>
<p><strong>Action</strong>:</p>
</li>
<li>
<p>Users choose a cryptocurrency network (chain) from a list provided in the app.</p>
</li>
<li>
<p>For each selected chain, the system creates a separate wallet, as required by blockchain protocols.</p>
</li>
<li>
<p>The wallet information, including wallet ID and balance, is securely stored in the user’s profile.</p>
</li>
<li>
<p><strong>User Interface Guidance</strong>:</p>
</li>
<li>
<p>Display a list of supported cryptocurrencies.</p>
</li>
<li>
<p>Provide clear instructions for setting up wallets.</p>
</li>
<li>
<p>Show wallet details such as balance and transaction history in an accessible format.</p>
</li>
</ul>
<h3 id="passphrase-security-for-wallets">3. Passphrase Security for Wallets</h3>
<ul>
<li>
<p><strong>Purpose</strong>: To protect user wallets and transactions, ensuring data privacy.</p>
</li>
<li>
<p><strong>Action</strong>:</p>
</li>
<li>
<p>During wallet setup, users create a secure passphrase.</p>
</li>
<li>
<p>The passphrase is encrypted and hashed, which means it cannot be accessed by anyone else, including the platform’s development team.</p>
</li>
<li>
<p><strong>User Interface Guidance</strong>:</p>
</li>
<li>
<p>Educate users about the importance of a secure passphrase and encourage unique, strong passphrases.</p>
</li>
<li>
<p>Notify users that the passphrase is encrypted for privacy, giving them peace of mind.</p>
</li>
</ul>
<h3 id="transactions-using-phone-number">4. Transactions Using Phone Number</h3>
<ol>
<li><strong>Initiating a Transaction</strong>:</li>
</ol>
<ul>
<li>
<p>Users select a recipient by entering their phone number.</p>
</li>
<li>
<p>They input the amount and select the cryptocurrency for the transaction.</p>
</li>
</ul>
<ol start="2">
<li><strong>Process</strong>:</li>
</ol>
<ul>
<li>
<p>The system checks if the recipient’s phone number is registered.</p>
</li>
<li>
<p>If the recipient is registered:</p>
</li>
<li>
<p>The transaction is processed, and both users receive notifications.</p>
</li>
<li>
<p>If the recipient is not registered:</p>
</li>
<li>
<p>The transaction is saved as “Pending” until the recipient registers.</p>
</li>
</ul>
<ol start="3">
<li><strong>User Interface Guidance</strong>:</li>
</ol>
<ul>
<li>
<p>Use intuitive prompts to guide users through each transaction step.</p>
</li>
<li>
<p>Display pending transactions prominently on the sender’s dashboard, especially for transactions awaiting recipient registration.</p>
</li>
</ul>
<h3 id="peer-to-peer-p2p-transactions">5. Peer-to-Peer (P2P) Transactions</h3>
<ol>
<li>
<p><strong>Purpose</strong>: Enable users to transfer cryptocurrency directly to other registered users.</p>
</li>
<li>
<p><strong>Process</strong>:</p>
</li>
</ol>
<ul>
<li>
<p>Users initiate a P2P transaction, similar to a bank transfer, which includes a small transaction fee for the platform.</p>
</li>
<li>
<p>Wallets are temporarily frozen during the transaction to ensure there are no disruptions, and the transaction is securely processed.</p>
</li>
</ul>
<ol start="3">
<li><strong>User Interface Guidance</strong>:</li>
</ol>
<ul>
<li>
<p>Provide an easily accessible “P2P Transaction” option.</p>
</li>
<li>
<p>Show real-time transaction confirmations and clear notifications for both sender and recipient.</p>
</li>
</ul>
<h3 id="buying-tokens-from-the-platform">6. Buying Tokens from the Platform</h3>
<ol>
<li>
<p><strong>Purpose</strong>: Allow users to buy cryptocurrency directly from within the app.</p>
</li>
<li>
<p><strong>How It Works</strong>:</p>
</li>
</ol>
<ul>
<li>
<p>The platform purchases the cryptocurrency from a third-party exchange (e.g., Luno) and resells it to users.</p>
</li>
<li>
<p>A small commission fee is included in the transaction to generate revenue.</p>
</li>
</ul>
<ol start="3">
<li><strong>User Interface Guidance</strong>:</li>
</ol>
<ul>
<li>
<p>Create a “Buy Crypto” section where users can view real-time prices and proceed with purchases.</p>
</li>
<li>
<p>Show users a clear breakdown of transaction fees and final prices for transparency.</p>
</li>
</ul>
<h3 id="wallet-freezing-during-transactions">7. Wallet Freezing During Transactions</h3>
<ul>
<li>
<p><strong>Purpose</strong>: Ensures security and transaction integrity.</p>
</li>
<li>
<p><strong>When</strong>:</p>
</li>
<li>
<p>During any active transaction, such as a transfer or P2P transaction, the wallet is temporarily frozen.</p>
</li>
<li>
<p>Additionally, if a user violates compliance criteria, their wallet may be frozen for security reasons.</p>
</li>
</ul>
<hr>
<h2 id="technical-concepts">Technical Concepts</h2>
<h3 id="wallet-architecture">Wallet Architecture</h3>
<ul>
<li>
<p><strong>Individual Wallets for Cryptocurrencies</strong>: Each cryptocurrency requires its own wallet due to blockchain and API limitations. Users wishing to transact with multiple coins will therefore need a separate wallet for each.</p>
</li>
<li>
<p><strong>Secure Storage</strong>: Wallets are stored with unique IDs and can be accessed only by authorized users through the API.</p>
</li>
</ul>
<h3 id="system-processes">System Processes</h3>
<ul>
<li>
<p><strong>Create Wallet</strong>:</p>
</li>
<li>
<p>When a user requests a wallet, the system generates it via API, storing the wallet details securely in the user’s profile.</p>
</li>
<li>
<p><strong>Create Address</strong>:</p>
</li>
<li>
<p>Users can request new addresses within a wallet, and the system will handle address generation through the API.</p>
</li>
<li>
<p><strong>Send Transaction</strong>:</p>
</li>
<li>
<p>For any initiated transaction, the system verifies the recipient’s details and processes the payment. The transaction status is tracked (e.g., pending, completed).</p>
</li>
<li>
<p><strong>Get Wallet Balance</strong>:</p>
</li>
<li>
<p>Users can retrieve real-time wallet balances on demand.</p>
</li>
</ul>
<hr>
<h2 id="example-system-actions">Example System Actions</h2>
<ol>
<li><strong>Pending Transactions for Unregistered Users</strong>:</li>
</ol>
<ul>
<li>The system periodically checks for new user registrations to match with pending transactions, automatically completing them when a match is found.</li>
</ul>
<ol start="2">
<li><strong>User Notifications</strong>:</li>
</ol>
<ul>
<li>Notifications should be integrated into the design to confirm transactions, update balances, and remind recipients about pending registrations.</li>
</ul>
<ol start="3">
<li><strong>Transaction History</strong>:</li>
</ol>
<ul>
<li>Display a transaction history that includes all pending, completed, and failed transactions to ensure transparency.</li>
</ul>
<hr>
<h2 id="visual-flowchart-of-the-process">Visual Flowchart of the Process</h2>
<p>Below is a <code>Mermaid</code> flowchart to visually map the entire process from selecting chains to wallet security, P2P transactions, and token purchases:</p>
<pre class=" language-mermaid"><svg id="mermaid-svg-1l08RAR6UPcP42pH" width="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" height="989.9140625" style="max-width: 1303.546875px;" viewBox="0 0 1303.546875 989.9140625"><style>#mermaid-svg-1l08RAR6UPcP42pH{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#000000;}#mermaid-svg-1l08RAR6UPcP42pH .error-icon{fill:#552222;}#mermaid-svg-1l08RAR6UPcP42pH .error-text{fill:#552222;stroke:#552222;}#mermaid-svg-1l08RAR6UPcP42pH .edge-thickness-normal{stroke-width:2px;}#mermaid-svg-1l08RAR6UPcP42pH .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg-1l08RAR6UPcP42pH .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg-1l08RAR6UPcP42pH .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg-1l08RAR6UPcP42pH .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg-1l08RAR6UPcP42pH .marker{fill:#666;stroke:#666;}#mermaid-svg-1l08RAR6UPcP42pH .marker.cross{stroke:#666;}#mermaid-svg-1l08RAR6UPcP42pH svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg-1l08RAR6UPcP42pH .label{font-family:"trebuchet ms",verdana,arial,sans-serif;color:#000000;}#mermaid-svg-1l08RAR6UPcP42pH .cluster-label text{fill:#333;}#mermaid-svg-1l08RAR6UPcP42pH .cluster-label span{color:#333;}#mermaid-svg-1l08RAR6UPcP42pH .label text,#mermaid-svg-1l08RAR6UPcP42pH span{fill:#000000;color:#000000;}#mermaid-svg-1l08RAR6UPcP42pH .node rect,#mermaid-svg-1l08RAR6UPcP42pH .node circle,#mermaid-svg-1l08RAR6UPcP42pH .node ellipse,#mermaid-svg-1l08RAR6UPcP42pH .node polygon,#mermaid-svg-1l08RAR6UPcP42pH .node path{fill:#eee;stroke:#999;stroke-width:1px;}#mermaid-svg-1l08RAR6UPcP42pH .node .label{text-align:center;}#mermaid-svg-1l08RAR6UPcP42pH .node.clickable{cursor:pointer;}#mermaid-svg-1l08RAR6UPcP42pH .arrowheadPath{fill:#333333;}#mermaid-svg-1l08RAR6UPcP42pH .edgePath .path{stroke:#666;stroke-width:1.5px;}#mermaid-svg-1l08RAR6UPcP42pH .flowchart-link{stroke:#666;fill:none;}#mermaid-svg-1l08RAR6UPcP42pH .edgeLabel{background-color:white;text-align:center;}#mermaid-svg-1l08RAR6UPcP42pH .edgeLabel rect{opacity:0.5;background-color:white;fill:white;}#mermaid-svg-1l08RAR6UPcP42pH .cluster rect{fill:hsl(210,66.6666666667%,95%);stroke:#26a;stroke-width:1px;}#mermaid-svg-1l08RAR6UPcP42pH .cluster text{fill:#333;}#mermaid-svg-1l08RAR6UPcP42pH .cluster span{color:#333;}#mermaid-svg-1l08RAR6UPcP42pH div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:12px;background:hsl(-160,0%,93.3333333333%);border:1px solid #26a;border-radius:2px;pointer-events:none;z-index:100;}#mermaid-svg-1l08RAR6UPcP42pH:root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}#mermaid-svg-1l08RAR6UPcP42pH flowchart-v2{fill:apa;}</style><g transform="translate(0, 0)"><marker id="flowchart-pointEnd" class="marker flowchart" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="userSpaceOnUse" markerWidth="12" markerHeight="12" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowMarkerPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker><marker id="flowchart-pointStart" class="marker flowchart" viewBox="0 0 10 10" refX="0" refY="5" markerUnits="userSpaceOnUse" markerWidth="12" markerHeight="12" orient="auto"><path d="M 0 5 L 10 10 L 10 0 z" class="arrowMarkerPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker><marker id="flowchart-circleEnd" class="marker flowchart" viewBox="0 0 10 10" refX="11" refY="5" markerUnits="userSpaceOnUse" markerWidth="11" markerHeight="11" orient="auto"><circle cx="5" cy="5" r="5" class="arrowMarkerPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></circle></marker><marker id="flowchart-circleStart" class="marker flowchart" viewBox="0 0 10 10" refX="-1" refY="5" markerUnits="userSpaceOnUse" markerWidth="11" markerHeight="11" orient="auto"><circle cx="5" cy="5" r="5" class="arrowMarkerPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></circle></marker><marker id="flowchart-crossEnd" class="marker cross flowchart" viewBox="0 0 11 11" refX="12" refY="5.2" markerUnits="userSpaceOnUse" markerWidth="11" markerHeight="11" orient="auto"><path d="M 1,1 l 9,9 M 10,1 l -9,9" class="arrowMarkerPath" style="stroke-width: 2; stroke-dasharray: 1, 0;"></path></marker><marker id="flowchart-crossStart" class="marker cross flowchart" viewBox="0 0 11 11" refX="-1" refY="5.2" markerUnits="userSpaceOnUse" markerWidth="11" markerHeight="11" orient="auto"><path d="M 1,1 l 9,9 M 10,1 l -9,9" class="arrowMarkerPath" style="stroke-width: 2; stroke-dasharray: 1, 0;"></path></marker><g class="root"><g class="clusters"></g><g class="edgePaths"><path d="M862.900390625,49.71875L862.900390625,53.885416666666664C862.900390625,58.052083333333336,862.900390625,66.38541666666667,862.900390625,74.71875C862.900390625,83.05208333333333,862.900390625,91.38541666666667,862.900390625,95.55208333333333L862.900390625,99.71875" id="L-Start-SelectChain" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-Start LE-SelectChain" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M862.900390625,141.4375L862.900390625,145.60416666666666C862.900390625,149.77083333333334,862.900390625,158.10416666666666,862.900390625,166.4375C862.900390625,174.77083333333334,862.900390625,183.10416666666666,862.900390625,187.27083333333334L862.900390625,191.4375" id="L-SelectChain-WalletSetup" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-SelectChain LE-WalletSetup" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M862.900390625,233.15625L862.900390625,237.32291666666666C862.900390625,241.48958333333334,862.900390625,249.82291666666666,862.9837239583334,258.2395833333333C863.0670572916666,266.65625,863.2337239583334,275.15625,863.3170572916666,279.40625L863.400390625,283.65625" id="L-WalletSetup-MainMenu" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-WalletSetup LE-MainMenu" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M805.5966679946202,358.0165898696203L693.6026920788503,373.9604394746836C581.6087161630802,389.90428907974683,357.6207643315401,421.7919882898734,245.62678841577005,456.3191712282701C133.6328125,490.8463541666667,133.6328125,528.0130208333334,133.6328125,546.5963541666666L133.6328125,565.1796875" id="L-MainMenu-P2PTransaction" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-MainMenu LE-P2PTransaction" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M809.5993489628586,362.01927083785864L742.2260199690487,377.29600694821556C674.852690975239,392.57274305857237,540.1060329876195,423.1262152792862,472.73270399380976,456.98628472297645C405.359375,490.8463541666667,405.359375,528.0130208333334,405.359375,546.5963541666666L405.359375,565.1796875" id="L-MainMenu-BuyTokens" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-MainMenu LE-BuyTokens" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M133.6328125,606.8984375L133.6328125,625.4817708333334C133.6328125,644.0651041666666,133.6328125,681.2317708333334,133.6328125,706.2083333333334C133.6328125,731.1848958333334,133.6328125,743.9713541666666,133.6328125,750.3645833333334L133.6328125,756.7578125" id="L-P2PTransaction-FreezeWallet" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-P2PTransaction LE-FreezeWallet" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M133.6328125,798.4765625L133.6328125,802.6432291666666C133.6328125,806.8098958333334,133.6328125,815.1432291666666,133.6328125,823.4765625C133.6328125,831.8098958333334,133.6328125,840.1432291666666,133.6328125,844.3098958333334L133.6328125,848.4765625" id="L-FreezeWallet-CompleteTransaction" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-FreezeWallet LE-CompleteTransaction" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M133.6328125,890.1953125L133.6328125,894.3619791666666C133.6328125,898.5286458333334,133.6328125,906.8619791666666,230.0224609375,917.8969680907966C326.412109375,928.9319570149264,519.19140625,942.6686015298528,615.5810546875,949.536923787316L711.970703125,956.4052460447792" id="L-CompleteTransaction-UnfreezeWallet" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-CompleteTransaction LE-UnfreezeWallet" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M842.470703125,955.2816349683759L917.9833984375,948.6005812236466C993.49609375,941.9195274789172,1144.521484375,928.5574199894586,1220.0341796875,914.2331370780627C1295.546875,899.9088541666666,1295.546875,884.6223958333334,1295.546875,869.3359375C1295.546875,854.0494791666666,1295.546875,838.7630208333334,1295.546875,823.4765625C1295.546875,808.1901041666666,1295.546875,792.9036458333334,1295.546875,775.390625C1295.546875,757.8776041666666,1295.546875,738.1380208333334,1295.546875,706.2083333333334C1295.546875,674.2786458333334,1295.546875,630.1588541666666,1295.546875,586.0390625C1295.546875,541.9192708333334,1295.546875,497.7994791666667,1232.3944286358103,460.55771980168976C1169.2419822716204,423.3159604367129,1042.937089543241,392.9522333734258,979.7846431790512,377.77036984178227L916.6321968148612,362.58850631013877" id="L-UnfreezeWallet-MainMenu" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-UnfreezeWallet LE-MainMenu" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M405.359375,606.8984375L405.359375,625.4817708333334C405.359375,644.0651041666666,405.359375,681.2317708333334,405.359375,706.2083333333334C405.359375,731.1848958333334,405.359375,743.9713541666666,405.359375,750.3645833333334L405.359375,756.7578125" id="L-BuyTokens-PurchaseFromExchange" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-BuyTokens LE-PurchaseFromExchange" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M405.359375,798.4765625L405.359375,802.6432291666666C405.359375,806.8098958333334,405.359375,815.1432291666666,457.2236328125,824.8342031176047C509.087890625,834.5251770685427,612.81640625,845.5737916370855,664.6806640625,851.0980989213568L716.544921875,856.6224062056283" id="L-PurchaseFromExchange-ResellToUser" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-PurchaseFromExchange LE-ResellToUser" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M955.263671875,854.6398523981915L997.4475911458334,849.4459707484929C1039.6315104166667,844.2520890987944,1123.9993489583333,833.8643257993972,1166.1832682291667,821.027214983032C1208.3671875,808.1901041666666,1208.3671875,792.9036458333334,1208.3671875,775.390625C1208.3671875,757.8776041666666,1208.3671875,738.1380208333334,1208.3671875,706.2083333333334C1208.3671875,674.2786458333334,1208.3671875,630.1588541666666,1208.3671875,586.0390625C1208.3671875,541.9192708333334,1208.3671875,497.7994791666667,1159.3296863929468,460.9727224612198C1110.2921852858938,424.145965755773,1012.2171830717874,394.612244011546,963.1796819647342,379.8453831394325L914.142180857681,365.07852226731904" id="L-ResellToUser-MainMenu" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-ResellToUser LE-MainMenu" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M820.5672625420044,372.9871844170044L795.5527969100036,386.435934930837C770.5383312780028,399.8846854446696,720.5094000140015,426.7821864723348,695.5782677153342,446.70749948616736C670.6471354166666,466.6328125,670.8138020833334,479.5859375,670.8971354166666,486.0625L670.98046875,492.5390625" id="L-MainMenu-ComplianceCheck" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-MainMenu LE-ComplianceCheck" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M670.98046875,680.5390625L670.8971354166666,686.8489583333334C670.8138020833334,693.1588541666666,670.6471354166666,705.7786458333334,682.4515815674472,718.4817708333334C694.2560277182278,731.1848958333334,718.0315866864556,743.9713541666666,729.9193661705694,750.3645833333334L741.8071456546834,756.7578125" id="L-ComplianceCheck-WalletActive" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-ComplianceCheck LE-WalletActive" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M738.6416886494443,612.8778426005557L783.9507561662036,630.4646084171297C829.259823682963,648.0513742337038,919.8779587164814,683.2249058668518,971.653212434593,707.2049008500926C1023.4284661527045,731.1848958333334,1036.360838555409,743.9713541666666,1042.8270247567611,750.3645833333334L1049.2932109581134,756.7578125" id="L-ComplianceCheck-FreezeForSecurity" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-ComplianceCheck LE-FreezeForSecurity" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M819.3803543453166,756.7578125L831.2681338294306,750.3645833333334C843.1559133135444,743.9713541666666,866.9314722817722,731.1848958333334,878.8192517658862,702.7317708333334C890.70703125,674.2786458333334,890.70703125,630.1588541666666,890.70703125,586.0390625C890.70703125,541.9192708333334,890.70703125,497.7994791666667,888.4716729762258,467.11393900294087C886.2363147024516,436.42839883921494,881.7655981549034,419.1771101784299,879.5302398811292,410.5514658480374L877.2948816073551,401.92582151764486" id="L-WalletActive-MainMenu" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-WalletActive LE-MainMenu" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M1091.4880390418866,756.7578125L1097.9542252432389,750.3645833333334C1104.420411444591,743.9713541666666,1117.3527838472955,731.1848958333334,1123.8189700486478,702.7317708333334C1130.28515625,674.2786458333334,1130.28515625,630.1588541666666,1130.28515625,586.0390625C1130.28515625,541.9192708333334,1130.28515625,497.7994791666667,1093.7244286547248,461.5096208244419C1057.1637010594495,425.21976248221716,984.042245868899,396.7598374644342,947.4815182736238,382.52987495554277L910.9207906783487,368.2999124466513" id="L-FreezeForSecurity-MainMenu" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-FreezeForSecurity LE-MainMenu" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path><path d="M849.5058996426449,401.92582151764486L847.103874702204,410.5514658480374C844.7018497617632,419.1771101784299,839.8977998808817,436.42839883921494,837.4957749404408,463.63737650294087C835.09375,490.8463541666667,835.09375,528.0130208333334,835.09375,546.5963541666666L835.09375,565.1796875" id="L-MainMenu-End" class=" edge-thickness-normal edge-pattern-solid flowchart-link LS-MainMenu LE-End" style="fill:none;" marker-end="url(#flowchart-pointEnd)"></path></g><g class="edgeLabels"><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(133.6328125, 453.6796875)"><g class="label" transform="translate(-56.20703125, -13.359375)"><foreignObject width="112.4140625" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">P2P Transaction</span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(405.359375, 453.6796875)"><g class="label" transform="translate(-39.05859375, -13.359375)"><foreignObject width="78.1171875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">Buy Tokens</span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(670.48046875, 718.3984375)"><g class="label" transform="translate(-68.8359375, -13.359375)"><foreignObject width="137.671875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">User Meets Criteria</span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(1010.49609375, 718.3984375)"><g class="label" transform="translate(-99.7890625, -13.359375)"><foreignObject width="199.578125" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">User Does Not Meet Criteria</span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g></g><g class="nodes"><g class="node default default" id="flowchart-Start-324" transform="translate(862.900390625, 28.859375)"><rect class="basic label-container" style="" rx="0" ry="0" x="-25.00390625" y="-20.859375" width="50.0078125" height="41.71875"></rect><g class="label" style="" transform="translate(-17.50390625, -13.359375)"><foreignObject width="35.0078125" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Start</span></div></foreignObject></g></g><g class="node default default" id="flowchart-SelectChain-325" transform="translate(862.900390625, 120.578125)"><rect class="basic label-container" style="" rx="0" ry="0" x="-130.8984375" y="-20.859375" width="261.796875" height="41.71875"></rect><g class="label" style="" transform="translate(-123.3984375, -13.359375)"><foreignObject width="246.796875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">User Selects Cryptocurrency Chain</span></div></foreignObject></g></g><g class="node default default" id="flowchart-WalletSetup-327" transform="translate(862.900390625, 212.296875)"><rect class="basic label-container" style="" rx="0" ry="0" x="-131.55859375" y="-20.859375" width="263.1171875" height="41.71875"></rect><g class="label" style="" transform="translate(-124.05859375, -13.359375)"><foreignObject width="248.1171875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Set Up Wallet &amp; Create Passphrase</span></div></foreignObject></g></g><g class="node default default" id="flowchart-MainMenu-329" transform="translate(862.900390625, 349.23828125)"><polygon points="66.08203125,0 132.1640625,-66.08203125 66.08203125,-132.1640625 0,-66.08203125" class="label-container" transform="translate(-66.08203125,66.08203125)" style=""></polygon><g class="label" style="" transform="translate(-37.72265625, -13.359375)"><foreignObject width="75.4453125" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Main Menu</span></div></foreignObject></g></g><g class="node default default" id="flowchart-P2PTransaction-331" transform="translate(133.6328125, 586.0390625)"><rect class="basic label-container" style="" rx="0" ry="0" x="-92.1875" y="-20.859375" width="184.375" height="41.71875"></rect><g class="label" style="" transform="translate(-84.6875, -13.359375)"><foreignObject width="169.375" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Initiate P2P Transaction</span></div></foreignObject></g></g><g class="node default default" id="flowchart-BuyTokens-333" transform="translate(405.359375, 586.0390625)"><rect class="basic label-container" style="" rx="0" ry="0" x="-121.12109375" y="-20.859375" width="242.2421875" height="41.71875"></rect><g class="label" style="" transform="translate(-113.62109375, -13.359375)"><foreignObject width="227.2421875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">User Buys Tokens from Platform</span></div></foreignObject></g></g><g class="node default default" id="flowchart-FreezeWallet-335" transform="translate(133.6328125, 777.6171875)"><rect class="basic label-container" style="" rx="0" ry="0" x="-125.6328125" y="-20.859375" width="251.265625" height="41.71875"></rect><g class="label" style="" transform="translate(-118.1328125, -13.359375)"><foreignObject width="236.265625" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Freeze Wallet During Transaction</span></div></foreignObject></g></g><g class="node default default" id="flowchart-CompleteTransaction-337" transform="translate(133.6328125, 869.3359375)"><rect class="basic label-container" style="" rx="0" ry="0" x="-85.16796875" y="-20.859375" width="170.3359375" height="41.71875"></rect><g class="label" style="" transform="translate(-77.66796875, -13.359375)"><foreignObject width="155.3359375" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Complete Transaction</span></div></foreignObject></g></g><g class="node default default" id="flowchart-UnfreezeWallet-339" transform="translate(777.220703125, 961.0546875)"><rect class="basic label-container" style="" rx="0" ry="0" x="-65.25" y="-20.859375" width="130.5" height="41.71875"></rect><g class="label" style="" transform="translate(-57.75, -13.359375)"><foreignObject width="115.5" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Unfreeze Wallet</span></div></foreignObject></g></g><g class="node default default" id="flowchart-PurchaseFromExchange-343" transform="translate(405.359375, 777.6171875)"><rect class="basic label-container" style="" rx="0" ry="0" x="-96.09375" y="-20.859375" width="192.1875" height="41.71875"></rect><g class="label" style="" transform="translate(-88.59375, -13.359375)"><foreignObject width="177.1875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Platform Buys from Luno</span></div></foreignObject></g></g><g class="node default default" id="flowchart-ResellToUser-345" transform="translate(835.904296875, 869.3359375)"><rect class="basic label-container" style="" rx="0" ry="0" x="-119.359375" y="-20.859375" width="238.71875" height="41.71875"></rect><g class="label" style="" transform="translate(-111.859375, -13.359375)"><foreignObject width="223.71875" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Resell to User with Commission</span></div></foreignObject></g></g><g class="node default default" id="flowchart-ComplianceCheck-349" transform="translate(670.48046875, 586.0390625)"><polygon points="94,0 188,-94 94,-188 0,-94" class="label-container" transform="translate(-94,94)" style=""></polygon><g class="label" style="" transform="translate(-65.640625, -13.359375)"><foreignObject width="131.28125" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Check Compliance</span></div></foreignObject></g></g><g class="node default default" id="flowchart-WalletActive-351" transform="translate(780.59375, 777.6171875)"><rect class="basic label-container" style="" rx="0" ry="0" x="-86.55078125" y="-20.859375" width="173.1015625" height="41.71875"></rect><g class="label" style="" transform="translate(-79.05078125, -13.359375)"><foreignObject width="158.1015625" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Wallet Remains Active</span></div></foreignObject></g></g><g class="node default default" id="flowchart-FreezeForSecurity-353" transform="translate(1070.390625, 777.6171875)"><rect class="basic label-container" style="" rx="0" ry="0" x="-101.1640625" y="-20.859375" width="202.328125" height="41.71875"></rect><g class="label" style="" transform="translate(-93.6640625, -13.359375)"><foreignObject width="187.328125" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">Freeze Wallet for Security</span></div></foreignObject></g></g><g class="node default default" id="flowchart-End-359" transform="translate(835.09375, 586.0390625)"><rect class="basic label-container" style="" rx="0" ry="0" x="-20.61328125" y="-20.859375" width="41.2265625" height="41.71875"></rect><g class="label" style="" transform="translate(-13.11328125, -13.359375)"><foreignObject width="26.2265625" height="26.71875"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="nodeLabel">End</span></div></foreignObject></g></g></g></g></g></svg></pre>
<hr>
</div>
</body>

</html>
