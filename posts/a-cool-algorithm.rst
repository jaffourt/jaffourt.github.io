.. title: A cool algorithm
.. slug: a-cool-algorithm
.. date: 2020-06-30 11:39:35 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
.. has_math: yes


This is a cool algorithm that I like. It is similar to a genetic algorithm but rather than updating the genes, you update the environment!

.. code-block:: python
		
   procedure ACO_MetaHeuristic is
       while not_termination do
           generateSolutions()
           daemonActions()
           pheromoneUpdate()
       repeat
   end procedure

The pheromoneUpdate() updates the environment, which optimizes other agents ability to solve some problem in said environment. The agents evaluate potential solutions, or rather perform an action governed by a probabilty distribution across available states. 

.. math::
   p^{k}_{xy} = \frac{(\tau^{\alpha}_{xy})(\eta^{\beta}_{xy})}{\sum_{z \in allowed_{x}}{(\tau^{\alpha}_{xy})(\eta^{\beta}_{xy})}}

Where :math:`\tau_{xy}` is the amount of pheromone between two states, :math:`x` and :math:`y`, and :math:`0<\alpha` controls the influence of of :math:`\tau_{xy}`. I like to think of this as an environmental factor that is uncontrollable to the agents. Maybe it is a windy day or it's raining, so the pheromones are difficult to detect!

And :math:`\eta_{xy}` is the desirability of a state transition between :math:`x` and :math:`y` (a priori knowledge of the states), and :math:`0<\beta` controls the influence of of :math:`\eta_{xy}`. Water is pretty undesirable to an agent without gills!

More on this soon...
