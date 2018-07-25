##############
ncview 使用说明
##############

*由北京朗润知天科技有限公司支持*

运行ncview
----------

.. code:: bash

   docker run  --rm \
          -v /tmp/.X11-unix:/tmp/.X11-unix \
          -e DISPLAY=unix$DISPLAY \
          -v $HOME/ncview/.ncviewrc:/home/ncview/.ncviewrc \
          -v `pwd`:/home/ncview \
          weatherhub/ncview \
          file_to_be_display.nc
           
.. image:: https://g.codefresh.io/api/badges/build?repoOwner=weatherlab&repoName=ncview&branch=master&pipelineName=ncview&accountName=weatherhub&type=cf-1
   :target: https://g.codefresh.io/repositories/weatherlab/ncview/builds?filter=trigger:build;branch:master;service:5a85d84dc2785f0001852f6e~ncview
