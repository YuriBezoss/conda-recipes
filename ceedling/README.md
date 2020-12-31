#
conda uninstall ceedling
conda deactivate
conda activate build
conda build .

#
conda activate test
conda install -c $HOME/.conda/envs/build/conda-bld/ ceedling
ceedling version

#
GlobalSignRootCA_R3.pem must be manually added to \Library\lib\ruby\2.7.0\rubygems\ssl_certs\index.rubygems.org
