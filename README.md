# custodianpolicies
Repository for custodian policies



# Execute as try
custodian run --dryrun -s . policy_name.yml


# Redirect output to s3

custodian run --output-dir s3://<my-bucket>/<my-prefix> <policyfile>.yml


# Send a mesagge to sqs and mail

custodian run -s . test-mailer.yml

# Execute and redirect try output to s3
custodian run --dryrun -s --output-dir s3://<my-bucket>/<my-prefix> <policyfile>.yml
custodian run --dryrun -s s3://cloudcustodianjh/ tag-audit-rei.yml
custodian run --dryrun -s s3://cloudcustodianjh/ ebsunattached.yml
custodian run --dryrun -s s3://cloudcustodianjh/ rdsconnections.yml


# Execute and redirect output to s3
custodian run -s --output-dir s3://<my-bucket>/<my-prefix> <policyfile>.yml
custodian run -s s3://cloudcustodianjh/ tag-audit-rei.yml
custodian run -s s3://cloudcustodianjh/ ebsunattached.yml
custodian run -s s3://cloudcustodianjh/ rdsconnections.yml
