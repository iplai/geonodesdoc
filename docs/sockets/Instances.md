
# Data socket Instances

> Inherits from gn.Geometry
  
<sub>go to [index](../index.md)</sub>



## Static methods

- [FromGeometries](#fromgeometries) : instances (Instances)
- [InstanceOnPoints](#instanceonpoints) : instances (Instances)

## Properties

- [domain_size](#domain_size) : instance_count (Integer)
- [instance_count](#instance_count) : instance_count (Integer)

## Methods

- [duplicate_instances](#duplicate_instances) : Sockets      [geometry (Geometry), duplicate_index (Integer)]
- [realize](#realize) : geometry (Geometry)
- [rotate](#rotate) : instances (Instances)
- [scale](#scale) : instances (Instances)
- [to_points](#to_points) : points (Points)
- [translate](#translate) : instances (Instances)

## InstanceOnPoints
```{eval-rst}

Geometry node [*Instance on Points*].


  Args:
    points: Points
    selection: Boolean
    instance: Geometry
    pick_instance: Boolean
    instance_index: Integer
    rotation: Vector
    scale: Vector
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Instances
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.InstanceOnPoints`
  
  
  Blender reference : `GeometryNodeInstanceOnPoints <https://docs.blender.org/api/current/bpy.types.GeometryNodeInstanceOnPoints.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.InstanceOnPoints(points=points, selection=selection, instance=instance, pick_instance=pick_instance, instance_index=instance_index, rotation=rotation, scale=scale, label=node_label, node_color=node_color)
    

```
## FromGeometries
```{eval-rst}

Geometry node [*Geometry to Instance*].


  Args:
    geometry: <m>Geometry
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Instances
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.GeometryToInstance`
  
  
  Blender reference : `GeometryNodeGeometryToInstance <https://docs.blender.org/api/current/bpy.types.GeometryNodeGeometryToInstance.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.GeometryToInstance(*geometry, label=node_label, node_color=node_color)
    

```
## domain_size
```{eval-rst}

Geometry node [*Domain Size*].



  Returns:
    Integer
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.DomainSize`
  
  - component = 'INSTANCES'
    
  Blender reference : `GeometryNodeAttributeDomainSize <https://docs.blender.org/api/current/bpy.types.GeometryNodeAttributeDomainSize.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.DomainSize(geometry=self, component='INSTANCES', label=f"{self.node_chain_label}.domain_size")
    

```
## instance_count
```{eval-rst}

Geometry node [*Domain Size*].



  Returns:
    Integer
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.DomainSize`
  
  - component = 'INSTANCES'
    
  Blender reference : `GeometryNodeAttributeDomainSize <https://docs.blender.org/api/current/bpy.types.GeometryNodeAttributeDomainSize.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.DomainSize(geometry=self, component='INSTANCES', label=f"{self.node_chain_label}.instance_count")
    

```
## rotate
```{eval-rst}

Geometry node [*Rotate Instances*].


  Args:
    selection: Boolean
    rotation: Vector
    pivot_point: Vector
    local_space: Boolean
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Instances
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.RotateInstances`
  
  
  Blender reference : `GeometryNodeRotateInstances <https://docs.blender.org/api/current/bpy.types.GeometryNodeRotateInstances.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.RotateInstances(instances=self, selection=selection, rotation=rotation, pivot_point=pivot_point, local_space=local_space, label=node_label, node_color=node_color)
    

```
## scale
```{eval-rst}

Geometry node [*Scale Instances*].


  Args:
    selection: Boolean
    scale: Vector
    center: Vector
    local_space: Boolean
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Instances
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.ScaleInstances`
  
  
  Blender reference : `GeometryNodeScaleInstances <https://docs.blender.org/api/current/bpy.types.GeometryNodeScaleInstances.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.ScaleInstances(instances=self, selection=selection, scale=scale, center=center, local_space=local_space, label=node_label, node_color=node_color)
    

```
## translate
```{eval-rst}

Geometry node [*Translate Instances*].


  Args:
    selection: Boolean
    translation: Vector
    local_space: Boolean
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Instances
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.TranslateInstances`
  
  
  Blender reference : `GeometryNodeTranslateInstances <https://docs.blender.org/api/current/bpy.types.GeometryNodeTranslateInstances.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.TranslateInstances(instances=self, selection=selection, translation=translation, local_space=local_space, label=node_label, node_color=node_color)
    

```
## realize
```{eval-rst}

Geometry node [*Realize Instances*].


  Args:
    legacy_behavior (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Geometry
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.RealizeInstances`
  
  
  Blender reference : `GeometryNodeRealizeInstances <https://docs.blender.org/api/current/bpy.types.GeometryNodeRealizeInstances.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.RealizeInstances(geometry=self, legacy_behavior=legacy_behavior, label=node_label, node_color=node_color)
    

```
## to_points
```{eval-rst}

Geometry node [*Instances to Points*].


  Args:
    selection: Boolean
    position: Vector
    radius: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Points
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.InstancesToPoints`
  
  
  Blender reference : `GeometryNodeInstancesToPoints <https://docs.blender.org/api/current/bpy.types.GeometryNodeInstancesToPoints.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.InstancesToPoints(instances=self, selection=selection, position=position, radius=radius, label=node_label, node_color=node_color)
    

```
## duplicate_instances
```{eval-rst}

Geometry node [*Duplicate Elements*].


  Args:
    selection: Boolean
    amount: Integer
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Sockets [geometry (Geometry), duplicate_index (Integer)]
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.DuplicateElements`
  
  - domain = 'INSTANCE'
    
  Blender reference : `GeometryNodeDuplicateElements <https://docs.blender.org/api/current/bpy.types.GeometryNodeDuplicateElements.html>`_
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.DuplicateElements(geometry=self, selection=selection, amount=amount, domain='INSTANCE', label=node_label, node_color=node_color)
    
```