# How to run  TF wrapper
#### Sample Run :: ./tf_run plan jupyterhub --portfolio studio --product search --environment dev --region us-west-2


                                         command, component, log_level, portfolio, product, environment, region

Source Python Code : https://github.com/beelit94/python-terraform/tree/master

Creating CLI app in Python:
https://click.palletsprojects.com/en/7.x/arguments/#arguments


extra_vars = {
    'pfolio': pfolio,
    'product': product,
    'environment': environment,
    'common_tags': {'Product': product, 'Pfolio': pfolio, 'Environment': environment}
}

additional_tf_args = {
    "capture_output": False,
    "var_file": [],
    "var": extra_vars
}
