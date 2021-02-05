local_resource(
  'apiserver',
  serve_cmd='make run-apiserver')

local_resource(
  'kubectl-get',
  cmd='kubectl --kubeconfig kubeconfig --username tilt --password dev api-resources',
  trigger_mode=TRIGGER_MODE_MANUAL,
  auto_init=False)

local_resource(
  'kubectl-apply',
  cmd='kubectl --kubeconfig kubeconfig --username tilt --password dev apply -f manifest.yaml -v 9',
  trigger_mode=TRIGGER_MODE_MANUAL,
  auto_init=False)
