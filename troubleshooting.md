# Troubleshooting

## Technical Knowledge and Skills

### Can you explain the steps you would take to troubleshoot a computer that won’t boot?

- Double check power source / try a new power source
- If tower is receiving power, check monitor connections
- Disconnect USB devices & try to boot
- Remove new hardware installed / Check it is installed correctly
- Listen for a POST beep (install a internal speaker if none installed)
- Use System Restore or Startup Repair
- Escalate via ticketing system if unable to solve

### How do you handle a situation where a user is unable to connect to the company’s VPN?

- Check Internet Connection
- Check your VPN credentials
- Restart any VPN software
- Check your VPN settings
- Clear old VPN software from device
- Reinstall / Update VPN software
- Reboot the router
- Try different VPN protocols/ports
- Escalate via ticketing system if unable to solve

### Describe the process of setting up a new user in a Windows environment

- Start > Settings > Accounts > Other Users > Add someone else to this PC

### What steps would you take to resolve a slow performance issue on a user’s computer?

- Check running tasks in Task Manager
- If Task Manager shows the issue - solve it either via ending the processes or uninstalling the problem application / adding more RAM / etc
- Restart PC
- Check disk space / free up disk space
- Update OS and Software
- Run a hardware diagnostic test
- Escalate via ticketing system if unable to solve

### How do you approach diagnosing a network connectivity problem?

- Figure out the exact problem being had (slow connection? no connection at all? connected locally but not to the internet?)
- Check all physical connections
- Restart computer / modem / router
- Run network diagnostics
- Disable firewalls / antivirus
- Test connection with a different device
- Escalate via ticketing system if unable to solve

## Problem-Solving and Analytical Skills

### Can you describe a time when you had to troubleshoot a particularly difficult technical issue? How did you resolve it?

- I often have to resolve difficult problems while independent broadcasting, one specific issue I remember having was constant dropped frames due to rendering & encoding lag. I tried a few solutions off the top of my mind that might work - dropping from 1080p to 720p for example worked well. But I didn't want to sacrifice quality! So I did more research with Google-fu and tested some more options presented by others having similar issues. Turned out - my CPU was too weak for the rendering / encoding I was trying to do! One great way to solve this was to upgrade to a 2000 series NVidia GPU - which gave me the option of NVENC encoding to off-load tons of the work onto my graphics card.

### If a user reports that their email client is not receiving emails, what steps would you take to resolve the issue?

- Double check they are connected to the internet
- Double check emails aren't going to spam
- Verify username & passwords are correct
- Check SMTP server details / change SMTP port
- Make sure firewalls & anti-virus aren't causing a conflict
- Send a test email and see if we receive a non-delivery report message
- Escalate via ticketing system if unable to solve

### How do you prioritize multiple IT support requests when they come in at the same time?

- I would quickly skim over each support request and see which one is causing barriers to peoples' immediate needs. After identifying which ones are causing barriers - I would pick the easiest fixes first so that those people could continue past their barrier. After which I would move on to the more difficult tickets and apologize for the wait.

## Customer Service and Communication

### Describe a situation where you had to explain a technical issue to a non-technical user. How did you ensure they understood?

- I often find myself having to explain independent broadcasting software to other aspiring broadcasters. This gives me a great chance to use non-techincal wording for a fairly technical software, and finding way to use non-technical words for tech jargon can actually be a fun challenge! It also helps me understand it better myself. One way I make sure they understood is asking them to repeat back what I explained to them in their own words & leave notes for them on any confusing parts.

### How would you handle a situation where a user is frustrated and upset about a recurring technical problem?

- First off, apologize! No one likes tech issues, and repeated ones can be annoying. I would also mention this is just the nature of computers sometimes - its not the user's fault! Afterwards, I would try to set them up in the best way possible for this technical problem to happen again - and if possible get them setup with an upgrade to completely solve it!

## Knowledge of Tools and Systems

### What ticketing systems have you used in the past, and how do you ensure that all relevant information is documented?

- I have used an in-house ticketing system built by CodeFellows within the application Remo. Students were able to input their current issue & location within Remo classroom. I always make sure to take notes when helping a student & keep track of any solutions we find to their issue. Afterwards, when closing the ticket, I place theses notes & any other important documentation in the closing remarks.

### How do you stay updated with the latest technology trends and advancements?

- Its a constant battle - but I am always trying to keep up with new YouTube videos, reading LinkedIn posts from other developers, and doing personal research for my own indepedent broadcasting and video game creation projects.

## Scenario-Based Questions

### A critical application is down, and multiple users are affected. Walk me through your process for handling this situation

- Communicate issue with users & let them know a solution is being worked on.
- Identify the issue at hand
- Restart the application
- Review available logs & error messages
- Look into recent updates or changes that could be reverted
- Communicate with other team members & escalate if we can't solve the issue
- Update users & management when solved, document solution
- Make sure it won't happen again by fixing whatever may have caused it

### You’ve identified a recurring issue with a particular software that affects many users. How would you go about addressing this on a larger scale?

- Document the issue as best as possible, creating a flow chart to recreate the issue if needed
- Inform team members of the issue, make sure there is not an easy solution I am missing
- Escalate to management & ask if I can help with a solution
- Research solutions to the issue & implement them as part of the software or procedure to use the software

## Technical Knowledge Verification

### Can you explain the difference between an incremental and a differential backup?

- Incremental only copies modified data since last backup. Ex: take a full backup on Sunday, your incremental backup on Monday will only contain changes since backup made on Sunday. Another incremental backup on Tuesday would only show changes since Monday.
- Differential copies only newly added and changed data since last FULL backup. Ex: take a full back up on Sunday, your differential backup on Monday will contain all data since Sunday. Another differntial backup on Tuesday will still contain all data since Sunday. Size of differential data will continue to increase until another full backup is completed.

### What is your experience with patch management, and how do you ensure systems remain secure and up-to-date?

- I have a fair amount of experience with patch management. One thing I find important is while keeping your systems up to date, automatic updates can sometimes be poorly timed. I like to do once a week regular checks on my systems to make sure all software used is updated. As for security - I think a good anti-virus and malware protection is important. Windows Defender will do the trick if you aren't downloading anything too risky & MalwareBytes has always worked well historically for me.

## Bonus Questions

### A user reports receiving “Page cannot be displayed,” troubleshooting procedure

- Ensure they are connected to the internet & other pages display
- Check this webpage loads on other devices and / or browsers
- If internet works on other sites and this webpage loads on other devices, clear cache & cookies is a great next step.
- Check DNS Settings / Flush DNS cache can always be a great next solution.

### Malware removal procedure, and common places for malware to hide

- Disconnect from internet
- Boot into Safe Mode
- Run a virus / malware scan
- Uninstall suspicious applications
- Delete suspicious browser extensions

### A user cannot log onto their workstation using their domain credentials, receiving “System could not log you on, make sure user name and domain are correct.”  Local user accounts log on successfully.  How can domain user log in?

- Make sure to be including the domain name correctly, show them how to do so.

### A user cannot access a network share.  Describe troubleshooting process for each:

- “Access is denied”

1. Check internet connection
2. Restart networking services
3. Make sure proper permissions are available to user & if not, help them get access

- “Network path was not found”

1. Double check path name
2. Try to connect using an IP address
3. Disable antivirus temporarily

### How can a domain user have the same network drive automatically mapped on any domain computer they log on to Multiple wireless access points are broadcasting the same SSID, one with encryption and one without.  Windows sees the network as encrypted.  How can you connect to the non-encrypted network?

- 

### A Windows installer does not detect a hard drive, describe possible scenarios which may cause this and possible solutions

- A few scenarios are loose/damaged cables, incompatible drivers, incorrect BIOS settings, faulty hard drive, unsupported hardware, or disk format/partition issues.

- Check that the Hard Drive shows up in the BIOS
- Double check all cables are snug, then replace cables if they look damaged at all.
- Try using a different port
- Connect hard drive to another PC to make sure it works
