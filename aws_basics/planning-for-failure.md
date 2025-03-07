# Planning For Failure

Backup plans for possible tragedies.

## Storage

When a file is stored in Amazon S3, the file is redundantly copied into every AZ in that Region. If one AZ goes down, you still have two copies of that file available for you.

## Compute

It's a best practice to spread out your computing resources across multiple AZs to guarantee high availability. So, if one AZ goes down, your architecture is still up and running.

## Database (db)

You can configure you db for Multi-AZ deployment. If your AZ with your primary db fails, one of the standby dbs in a healthy AZ automatically becomes your new primary database.

Therefore, your architecture is still running.
