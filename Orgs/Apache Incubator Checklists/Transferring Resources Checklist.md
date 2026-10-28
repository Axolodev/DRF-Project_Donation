
*Retrieved from https://incubator.apache.org/guides/transferring.html* 

- Update the Incubator status records
    
    - Like the rest of incubation, graduation is a process. Updating your status records as you progress will enable others to assist.
        
    - Update the podling status page. All sections should now be filled in including **EXIT**. Take some time to read carefully since this page forms the final public record for graduation.
        
    
- Source
    
    - SVN repositories will be moved from the incubator to other locations, if you need the move done please raise an infra ticket after the TLP Parent Request.
        
    - Post an announcement to the development list telling everyone that the repository is about to be moved
        
    - Post an announcement containing instructions for developers describing how to ==svn switch== their workspaces
        
    - Update site, jenkins, wikis, **pom.xml** and other resources to point to the new repository location.
        
    
- Websites
    
    - Since podlings receive standard domains, no changes are required
        
    - Once graduated, your website will automatically redirect to remove the **incubator** subdomain
        
    - If you have any fully qualified links to your **podling.incubator.apache.org** on your website change them
        
    
- Mailing lists
    
    - Mailing lists no longer need to get moved, since podlings are given standard domains.
        
    - If you use **podling.incubator.apache.org** format email addresses, please start using **podling.apache.org**
        
    - When using Maven: update **pom.xml** for the new mailing list address(es). Also update any documents on your website that show how to subscribe to the lists and/or find archives.
        
    - Check project-private mailing list membership. Mentors should be allowed to remain if they wish to do so. The subscriber list should otherwise match that on the resolution. See [this](http://www.apache.org/dev/committers.html#mail-moderate) and the [EZMLM](http://www.ezmlm.org/) "Moderator’s and Administrator’s Manual".
        
    - Update mail addresses including:
        
        - confluence commit messages (see adminstration documentation)
            
        - issue tracking messages (see administration documentation)
            
        - The chair should have karma to perform these tasks.
            
        
    - Double-check that all of your lists have sufficient active [moderators](http://www.apache.org/dev/committers.html#mailing-list-moderators).
        
    
- Issue Tracking
    
    - Ask infra to move the podling to its own top level category in JIRA, if using JIRA
        
    
- Distribution mirrors
    
    - Dist area (dist.apache.org) **release/${project}** and **dev/${project}** folders can be created by PMC members.
        
        - Do not forget to copy KEYS file from **release/incubator/${project}** location.
            
        - You have two major options then:
            
            - you can **keep** incubating released artifacts at **release/incubator/${project}** and remove artifacts once your TLP project does their first release.
                
                File a JIRA under your newly JIRA **${project}** space to remind to remove **/dist/incubator/${project}/** after the first release in **/dist/${project}/**
                
            - you can **move** the last incubating released artifacts to your **release/${project}**, taking care that incubating stay in path (you will need to change website and mail for the new location)