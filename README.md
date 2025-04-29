# codes_scripts# Get the current timestamp
time_m = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")

# Get path and normalize ()windows 7 Linux ) using OS
raw_path = "C:\MohammadMofassairHos\OneDrive\test.txt"
dp_xls_path = os.path.normpath(raw_path)  # Normalize path separators

# Use variable within variable
_source = "loc_xls"  # loc_xls, db_os, db_influx
print(f"printing source: {config['dp_source']['loc_xls']['path']}")
print(f"printing source: {config['dp_source'][_source]['path']}")
