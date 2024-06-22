
A cool template to sign SparkOS builds with `dev-keys`.

## Usage

1. Clone the repository 

```
git clone https://github.com/jignesh2320/android_vendor_spark_priv.git vendor/spark-priv/keys 
```

2. Go to the key directory 

```
cd vendor/spark-priv/keys
```

3. Run the script

```
./gen_keys
```

It will generate the certificates in vendor/spark-priv/keys and the actual keys used to generate the certificates in ~/.android-certs/.

It will also generate the makefiles based on the keys defined in the _data/ folder.

Backup AT ALL COSTS your ~/.android-certs/ and vendor/spark-priv/keys folders AND NEVER LEAK THOSE. Losing these keys could prevent you from updating your SuperiorOS builds with the same keys, so formatting data would be required. Leakage of these keys can compromise the security and authenticity of your builds, requiring a new pair of keys to be generated.