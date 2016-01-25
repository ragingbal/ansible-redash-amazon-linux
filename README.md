# Ansible to deploy redash and mysql to Amazon Linux

# How to use

1. create Amazon Linux on EC2
2. change hosts with your EC2 global ip
3. ansible-playbook site.yml --private-key=~/.ssh/your-private-key.pem -u ec2-user -i hosts

Sometimes, there is an error, but you can re-run the 3rd step again to solve the problem.

After installing redash, you can access it with the EC2 global ip by browser.
The account/password are admin/admin.

MySQL account/password are analytics/analytics. 
MySQL dataset is imported to world database. 

Now you can import any data to MySQL to analyze your data!

# Dependent Roles

    geerlingguy.mysql    
    
