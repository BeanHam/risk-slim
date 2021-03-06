risk-slim
========

`risk-slim` is a machine learning method to create customized risk scores in python. 

### Background 

Risk scores are simple tools that let users make quick risk predictions by adding and subtracting a few small numbers (see e.g., medical risk scores at [www.mdcalc.com](https://www.mdcalc.com/) or the [mdcalc iOS app](https://itunes.apple.com/us/app/mdcalc-medical-calculators-clinical-scores/id1001640662?ls=1&mt=8)).

#### Video

<p align="center">
	<a href="http://www.youtube.com/watch?feature=player_embedded&v=WQDVejk17Aw" target="_blank">
		<img src="http://img.youtube.com/vi/WQDVejk17Aw/0.jpg" alt="RiskSLIM KDD" width="480" height="360" border="10" />
	</a>
</p>

#### Customized Risk Score for ICU seizure prediction 

Here is a risk score for ICU risk prediction that is described in our [paper](http://www.berkustun.com/docs/ustun_2017_optimized_risk_scores.pdf). 

<div>
<p align="center">
<img src="https://github.com/ustunb/risk-slim/blob/master/images/risk_score_seizure.png" width="480" height="360" border="0"/>
</p>
</div>

#### Paper

If you use ``risk-slim`` for in your research, please cite [our paper](http://www.berkustun.com/docs/ustun_2017_optimized_risk_scores.pdf):
     
```
@inproceedings{ustun2017kdd,
	Author = {Ustun, Berk and Rudin, Cynthia},
	Booktitle = {Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining},
	Organization = {ACM},
	Title = {{Optimized Risk Scores}},
	Year = {2017}}
}
```

## Package Details

**NOTE: THIS PACKAGE IS CURRENTLY UNDER DEVELOPMENT. THE CODE MAY CHANGE WITH EACH COMMIT.** 

### Installation
  
Run the following snippet to install ``risk-slim`` in a Mac/Unix environment, and complete a test run.  

```
git clone https://github.com/ustunb/risk-slim
cd risk-slim
pip install -e . #install in editable mode  
bash batch/job_template.sh #batch run
```

### Requirements

- Python 3.5+ 
- CPLEX 12.6+
 
The code may still work with older versions of Python and CPLEX, but this will not be tested or supported. If you're hesitant about switching to Python 3, check out this [migration guide](https://github.com/arogozhnikov/python3_with_pleasure) 

#### CPLEX 

CPLEX is cross-platform commercial optimization tool with a Python API. It is free for students and faculty members at accredited institutions. To get CPLEX:

1. Register for [IBM OnTheHub](https://ibm.onthehub.com/WebStore/Account/VerifyEmailDomain.aspx)
2. Download the *IBM ILOG CPLEX Optimization Studio* from the [software catalog](https://ibm.onthehub.com/WebStore/ProductSearchOfferingList.aspx?srch=CPLEX)
3. Install the CPLEX Optimization Studio.
4. Setup the CPLEX Python API [as described here](https://www.ibm.com/support/knowledgecenter/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html).

If you have problems installing CPLEX, check the [CPLEX user manual](http://www-01.ibm.com/support/knowledgecenter/SSSA5P/welcome) or the [CPLEX forums](https://www.ibm.com/developerworks/community/forums/html/forum?id=11111111-0000-0000-0000-000000002059). 

## Development Roadmap

**If you are interested in contributing, please reach out!**

- ~~simplify installation~~ 
- ~~convenience functions for batch computing~~
- ~~refactoring package for future development~~
- [sci-kit learn](http://scikit-learn.org/stable/developers/contributing.html#rolling-your-own-estimator) API (as of 10/11/2018)
- reporting tools (roc curves, calibration plots, model reports)
- support for open source solver
- documentation

