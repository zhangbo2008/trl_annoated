# trl_annoated



三个部分:
    1. trainer/sft_trainer.py:
        继承了trainer类.
        负对数似然损失(Negative Log-Likelihood Loss,简称NLL Loss)是常用的损失函数 在这个问题上等价于交叉熵.
        只需要我们设置好任务是causual_lm, 就可以自动进行学习.
        所以核心代码只有  
        def _prepare_dataset这个函数.


