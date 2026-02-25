# Commands Executed

## Initial Investigation

k get po



k get cm



k get cm nginx-config -o yaml

## Export Current Configuration

k get po nginx-phpfpm -o yaml > pod.yaml

## Rectify Mount Path Errors

vi pod.yaml

## Modify the mountPath to /var/www/html

## Rectify Mount Path Errors

k delete po nginx-phpfpm



k apply -f pod.yaml

## Verify Pod Readiness

k get po

## Copy Application Code

k cp index.php nginx-phpfpm:/var/www/html -c nginx-container



