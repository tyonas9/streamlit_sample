### Instructions on how to run it locally



### Deploy streamlit App on AWS EC2
1. Create an AWS account
2. Create an EC2 instance 
3. Configure custom TCP ports 8501/2
4. SSH into the instance 
    1. chmod 400 "name of private key/.pem"
    2. ssh -i "privatekey.pem" ec2-user@"PUBLICDNS(ipv4)"
    3. Install newer version of python on AWS : sudo yum install python36
    4. Install git : sudo yum install git
    5. Install streamlit : sudo python3.6 -m pip install streamlit
5. Run 
    1. From the application folder, to run use the command : steamlit run main.py
6. Use Tmux to keep it running 
    1. Install tmux : sudo yum install tmux
    2. crate a new tmux session : tmux new -s streamlitinstance 
    3. run the app in the tmux session : streamlit run main.py






