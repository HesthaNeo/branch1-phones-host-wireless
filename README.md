<p align="center">
<img width="656" height="209" alt="Screenshot 2026-04-16 233649" src="https://github.com/user-attachments/assets/0aea22f3-49f3-4add-941c-cafcb1febb35" />
</p>
<h1><u>Milestone 10: Branch 1 Phones, Hosts and Wireless</u></h1>
    <p>Ninth phase, we will install Cisco CP-7960 VoIP phones, connect host computers for testing, and also install 1 wireless access point for corporate network access using a unique SSID.</p>
    <h2><strong><u>Configuration Steps</u></strong></h2>
    <p><b>Step 1: Connect Two Cisco 7960 VoIP Phones To The Branch 1 Access Switch</b></p>
    <p><b>Step 2: Access The Branch 1 Router CLI And View The DHCP Bindings For Each Phone, Obtaining The MAC-Address Of Each Phone</b></p>
    <p><b>Step 3: On The Branch 1 Voice Router Configure The Two Ephones That Were Just Connected</b></p>
        <p>- A. Ephone 1, Ephone 2</p>
        <p>- B. MAC-Address</p>
        <p>- C. Phone Type</p>
        <p>- D. Button 1</p>
    <p><b>Step 4: Test Dialing By Extension Between Each Branch Phone And To The HQ Phones</b></p>
    <p><b>Step 5: Test Outbound Dialing To The PSTN Test Phone 8885551111</b></p>
    <p><b>Step 6: Test Inbound Dialing To B1 External Phone Number(s) <em>(Lab Configuration Not Supported)</em></b></p>
    <p><b>Step 7: Connect A Host Directly To Each Of The Two Cisco 7960 VoIP Phones That Were Just Connected To The Network</b></p>
    <p><b>Step 8: Test Each Host By Pinging Around The Branch 1 Network From Each Host, Between Each Host And To The Headquarters Network And PCs</b></p>
    <p><b>Step 9: Test IP Connectivity To The Internet By Pinging Google Server 8.8.8.8</b></p>
    <p><b>Step 10: Test DNS And Website Connectivity By Using The Web Browser On Each Host To Access Www.Google.Com</b></p>
    <p><b>Step 11: Install And Configure Corporate Wireless Access</b></p>
        <p>- A. Install An AccessPoint-PT And Connect It To The Branch 1 Access Switch</p>
        <p>- B. Configure The New AP With A uUnique SSID, Channel, And Passphrase Using WPA2-PSK And AES</p>
        <p>- C. Install Two Wireless Tablets And Configure Them With The Same SSID And Passphrase</p>
        <p>- D. Once The New Wireless Tablets Are Connected Confirm Access To The Corporate Networks And Internet</p>
        <h2><strong><u>Implementation</u></strong></h2>
        <h3>Step 1: Connect Two Cisco 7960 VoIP Phones To The Branch 1 Access Switch</h3>
                <img width="762" height="495" alt="Screenshot 2026-04-16 235639" src="https://github.com/user-attachments/assets/b0152e06-0733-41ba-a312-6724b8e19e45" />
        <h3>Step 2: Access The Branch 1 Router CLI And View The DHCP Bindings For Each Phone, Obtaining The MAC-Address Of Each Phone</h3>
                <img width="869" height="240" alt="Screenshot 2026-04-16 235828" src="https://github.com/user-attachments/assets/9eca259a-b329-42ac-b1d5-f0bd2e494139" />
        <h3>Step 3: On The Branch 1 Voice Router Configure The Two Ephones That Were Just Connected</h3>
                <img width="873" height="823" alt="Screenshot 2026-04-17 000034" src="https://github.com/user-attachments/assets/6721d78a-fd6f-4700-91c2-5f687d5cf919" />
        <h3>Step 4: Test Dialing By Extension Between Each Branch Phone And To The HQ Phones</h3>
                <img width="1749" height="886" alt="Screenshot 2026-04-17 000337" src="https://github.com/user-attachments/assets/a7713800-c59d-4724-9d8a-0683ba0415eb" />
                <p><em>- We are able to successfully place calls between the branch 1 phones.</em></p>
                <img width="1748" height="883" alt="Screenshot 2026-04-17 001240" src="https://github.com/user-attachments/assets/d4928e98-fc49-40cb-bc05-5d7f9b35001f" />
                <p><em>- We are able to successfully place calls to the HQ from branch 1.</em></p>
        <h3>Step 5: Test Outbound Dialing To The PSTN Test Phone 8885551111</h3>
                <img width="1739" height="880" alt="Screenshot 2026-04-17 000508" src="https://github.com/user-attachments/assets/bc927172-781e-4db3-b9eb-b77c1c7c7c6a" />
                <p><em>- We are able to successfully place calls to the PSTN.</em></p>
        <h3>Step 6: Test Inbound Dialing To B1 External Phone Number(s) <em>(Lab Configuration Not Supported)</em></h3>
        <h3>Step 7: Connect A Host Directly To Each Of The Two Cisco 7960 VoIP Phones That Were Just Connected To The Network</h3>
                <img width="758" height="494" alt="Screenshot 2026-04-17 001606" src="https://github.com/user-attachments/assets/283ea139-330f-4d65-b754-ab8d70d7a616" />
        <h3>Step 8: Test Each Host By Pinging Around The Branch 1 Network From Each Host, Between Each Host And To The Headquarters Network And PCs</h3>
                <img width="872" height="1318" alt="Screenshot 2026-04-17 001920" src="https://github.com/user-attachments/assets/a1d7a9e8-b075-44c8-a06f-548d7253e0e1" />
                <img width="872" height="1316" alt="Screenshot 2026-04-17 002041" src="https://github.com/user-attachments/assets/49211c4c-7f85-4f2f-9b20-12b7b72fba30" />
                <p><em>- On both hosts we are able to successfully ping 192.168.20.1 (default gateway), 192.168.10.100 (the HQ-Core Switch Data network gateway at HQ), 192.168.10.50 (the HQ-Server), and both google's DNS server by IP and hostname.</em></p>
        <h3>Step 10: Test DNS And Website Connectivity By Using The Web Browser On Each Host To Access Www.Google.Com</h3>
                <img width="524" height="682" alt="Screenshot 2026-04-17 002316" src="https://github.com/user-attachments/assets/68e5ff3c-5682-40d6-a405-f14f3c521d80" />
                <img width="560" height="715" alt="Screenshot 2026-04-17 002346" src="https://github.com/user-attachments/assets/468b30ed-2d5f-4be9-bb11-9aff0185baee" />
                <p><em>- Successful.</em></p>
        <h3>Step 11: Install And Configure Corporate Wireless Access</h3>
            <p>- A. Install An AccessPoint-PT And Connect It To The Branch 1 Access Switch</p>
            <p>- B. Configure The New AP With A uUnique SSID, Channel, And Passphrase Using WPA2-PSK And AES</p>
            <p>- C. Install Two Wireless Tablets And Configure Them With The Same SSID And Passphrase</p>
            <p>- D. Once The New Wireless Tablets Are Connected Confirm Access To The Corporate Networks And Internet</p>









 





