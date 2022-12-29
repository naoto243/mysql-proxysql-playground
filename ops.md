

# ProxySQL用のmonitor userを用意する
CREATE USER IF NOT EXISTS 'monitor'@'%' IDENTIFIED BY 'monitor';
SET PASSWORD FOR monitor = 'proxysqlmonitor'