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
            <p>- A. First, we will rack, mount, and power on the cisco 2911 router.</p>
                <img width="1395" height="873" alt="Screenshot 2026-04-16 161350" src="https://github.com/user-attachments/assets/721ece10-de94-4c77-92cd-9dfc35198b4b" />
            <p>- B. Next, we will install the uck9 license.</p>
                <img width="866" height="995" alt="Screenshot 2026-04-16 161731" src="https://github.com/user-attachments/assets/7afcbaa1-7742-4097-b7c1-fc429f8569d0" />
                <img width="870" height="1137" alt="Screenshot 2026-04-16 161850" src="https://github.com/user-attachments/assets/52ae8506-d271-499e-9370-496677da66cd" />
                <img width="871" height="1354" alt="Screenshot 2026-04-16 161944" src="https://github.com/user-attachments/assets/377ce501-7d58-4aba-9849-8ea7e602f504" />
                <img width="872" height="1217" alt="Screenshot 2026-04-16 162032" src="https://github.com/user-attachments/assets/b597394e-aaee-4a8e-beaf-6bd237de2906" />
            <p>- C. Next we will do basic Router configurations (hostname, NTP, domain-name, SSH, etc).</p>
                <img width="874" height="968" alt="Screenshot 2026-04-16 162754" src="https://github.com/user-attachments/assets/3e343fe9-285e-4a55-89e8-875eee416989" />
            <p>- D. Now, we'll configure and connect branch 1 LAN interface G0/0. We'll set our VLANS respectively as well. (Mgmt interface vlan 100, data interface vlan 192, voice interface vlan 10.)</p>
                <img width="869" height="887" alt="Screenshot 2026-04-16 163432" src="https://github.com/user-attachments/assets/c0710a87-16ea-4e29-9e90-a407b5486548" />
        <h3>Step 4: Test Dialing By Extension Between Each Branch Phone And To The HQ Phones</h3>
            <p>- A. We'll start by racking, mounting, and powering on the branch 1 2960 switch.</p>
                <img width="1281" height="906" alt="Screenshot 2026-04-16 175802" src="https://github.com/user-attachments/assets/52b16c9b-2b4b-4f7a-ad8f-78c51d8dfa15" />
            <p>- B. Next we will do basic switch configurations (hostname, NTP, domain-name, SSH, etc).</p>
                <img width="872" height="979" alt="Screenshot 2026-04-16 180031" src="https://github.com/user-attachments/assets/939ab7dc-26f3-49e1-9910-b598ede5874d" />
            <p>- C. Next we will configure VLAN trunking protocol (VTP) transparent.</p>
                <img width="871" height="526" alt="Screenshot 2026-04-16 180520" src="https://github.com/user-attachments/assets/cdf6e515-4375-4ed3-95c7-a975f3b8549f" />
            <p>- D. Next, we'll configure MGMT vlan interface and add the voice and data vlans to the switch.</p>
                <img width="870" height="598" alt="Screenshot 2026-04-16 180841" src="https://github.com/user-attachments/assets/d1a9ed83-c8ce-4c20-9d1a-4a1eeff19b73" />
            <p>- E. *See last step*</p>
            <p>- F. Now we'll configure and connect trunks port back to the branch 1 router.</p>
                <img width="872" height="335" alt="Screenshot 2026-04-16 181154" src="https://github.com/user-attachments/assets/82b004e3-2cbc-4f32-b00a-7c9a2f64f9fd" />
                <img width="1151" height="902" alt="Screenshot 2026-04-16 181256" src="https://github.com/user-attachments/assets/1faa7292-5820-4bc6-9097-2bb8dc4625b8" />
            <p>- G. Lastly, we'll configure the access ports on the branch 1 switch.</p>
                <img width="869" height="1505" alt="Screenshot 2026-04-16 181544" src="https://github.com/user-attachments/assets/86663e80-8a33-45b4-a758-4d2716d714bf" />
                <img width="870" height="666" alt="Screenshot 2026-04-16 181634" src="https://github.com/user-attachments/assets/cbf22726-96c5-4d47-9c1b-40b024877f36" />
                <p><em>- *Now that the Branch 1 router and switch are installed, we can set up the phones, hosts & wireless!</em></p>
        <h3>Step 5: Test Outbound Dialing To The PSTN Test Phone 8885551111</h3>
        <h3>Step 6: Test Inbound Dialing To B1 External Phone Number(s) <em>(Lab Configuration Not Supported)</em></h3>
        <h3>Step 7: Connect A Host Directly To Each Of The Two Cisco 7960 VoIP Phones That Were Just Connected To The Network</h3>
        <h3>Step 8: Test Each Host By Pinging Around The Branch 1 Network From Each Host, Between Each Host And To The Headquarters Network And PCs</h3>
        <h3>Step 9: Test IP Connectivity To The Internet By Pinging Google Server 8.8.8.8</h3>
        <h3>Step 10: Test DNS And Website Connectivity By Using The Web Browser On Each Host To Access Www.Google.Com</h3>
        <h3>Step 11: Install And Configure Corporate Wireless Access</h3>
            <p>- A. Install An AccessPoint-PT And Connect It To The Branch 1 Access Switch</p>
            <p>- B. Configure The New AP With A uUnique SSID, Channel, And Passphrase Using WPA2-PSK And AES</p>
            <p>- C. Install Two Wireless Tablets And Configure Them With The Same SSID And Passphrase</p>
            <p>- D. Once The New Wireless Tablets Are Connected Confirm Access To The Corporate Networks And Internet</p>









 





