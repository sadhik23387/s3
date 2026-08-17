#!/bin/bash

echo "======================================"
echo "       LINUX SYSTEM HEALTH MONITOR"
echo "======================================"

echo ""
echo "Hostname:"
hostname

echo ""
echo "System Uptime:"
uptime

echo ""
echo "Memory Usage:"
free -h

echo ""
echo "Disk Usage:"
df -h

echo ""
echo "Top 5 CPU Processes:"
ps aux --sort=-%cpu | head -5

echo ""
echo "Top 5 Memory Processes:"
ps aux --sort=-%mem | head -6

echo ""
echo "Network Information:"
ip -brief addr

echo ""
echo "======================================"
echo "          HEALTH CHECK COMPLETE"
echo "======================================"
