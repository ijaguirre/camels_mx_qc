# Fir

>> Load modules 
ml load CCconfig gentoo/2023 StdEnv/2023 gcccore/.12.3 gcc/12.3 hwloc/2.9.1 ucx/1.14.1 libfabric/1.18.0 pmix/4.2.4 ucc/1.2.0 openmpi/4.1.5 flexiblas/3.3.1 aocl-blas/5.1 aocl-lapack/5.1 python/3.11.5 hdf5/1.14.2 netcdf/4.9.2 netcdf-fortran/4.6.1 openblas/0.3.24 hdf/4.2.16 jasper/4.0.0 proj/9.2.0 libgeotiff/1.7.1 libspatialindex/1.9.3 mpi4py/4.0.3 boost/1.82.0 eigen/3.4.0 arpack-ng/3.9.1 armadillo/12.6.4 cfitsio/4.3.0 postgresql/16.0 freexl/2.0.0 brunsli/0.1 qhull/2020.2 lerc/4.0.0 librttopo/1.1.0 libspatialite/5.1.0 gdal/3.9.1 geos/3.12.0 pnetcdf/1.12.3 yaxt/0.10.0 libaec/1.0.6 eccodes/2.31.0 fftw/3.3.10 udunits/2.2.28 cdo/2.2.2 antlr/2.7.7 libdap/3.20.11 gsl/2.7 nco/5.1.7

ml save camelsmx

ENV_DIR="/home/$USER/envs/camels_mx_env1"
echo "=== Creating virtual environment ==="
mkdir -p "$(dirname "$ENV_DIR")"
python -m venv "$ENV_DIR"
source "$ENV_DIR/bin/activate"
=== Creating virtual environment ===

python -m pip install \
    asttokens==3.0.2 \
    comm==0.2.3 \
    contourpy==1.3.3 \
    cramjam==2.14.0 \
    cycler==0.12.1 \
    debugpy==1.8.22 \
    executing==2.3.0 \
    fastparquet==2026.9.0 \
    fonttools==4.68.0 \
    fsspec==2026.9.0 \
    ipykernel==7.4.0 \
    ipython==9.18.1 \
    ipython_pygments_lexers==1.1.1 \
    jedi==0.20.1 \
    jupyter_client==8.10.0 \
    jupyter_core==5.9.1 \
    kiwisolver==1.5.1 \
    matplotlib==3.11.2 \
    matplotlib-inline==0.2.2 \
    nest-asyncio2==1.7.4 \
    numpy==2.3.3 \
    packaging==26.3 \
    pandas==3.0.5 \
    parso==0.8.7 \
    pexpect==4.9.0 \
    pip==24.0 \
    platformdirs==4.14.5 \
    prompt_toolkit==3.0.53 \
    psutil==7.2.2 \
    ptyprocess==0.7.0 \
    pure_eval==0.2.4 \
    Pygments==2.21.0 \
    pyparsing==3.3.3 \
    python-dateutil==4.0.0 \
    pyzmq==27.3.0 \
    scipy==1.17.1 \
    setuptools==65.5.0 \
    stack-data==0.6.3 \
    tornado==6.6.1 \
    traitlets==5.16.1 \
    typing_extensions==4.16.0 \
    tzdata==2026.6 \
    wcwidth==0.9.4

pip install cfgrib  click eccodes blosc2

python -m ipykernel install --name "camels_mx_env1" --user

